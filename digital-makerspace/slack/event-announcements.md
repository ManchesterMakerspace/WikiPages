---
title: Event announcements
description: Eventbrite announcements, reminders and ticket totals in Slack.
published: true
date: 2026-11-15T00:00:00.000Z
tags: slack, eventbrite
editor: markdown
dateCreated: 2026-11-15T00:00:00.000Z
---

# Event announcements

Public listed Eventbrite events appear in #upcoming-events, unless an administrator
has chosen another **Upcoming Events Channel** in Portal Settings → Slack.
The message shows the date, location, ticket totals and registration link.
Free admission tickets count too. Ticket totals are snapshots; Eventbrite remains
the source for current registration availability.

A recurring series receives one initial announcement for its first upcoming date.
Upcoming reminders group the series' dates and show ticket totals separately.
There is at most one reminder per event or series per Eastern calendar day.
Running a wider reminder window later that day adds dates to the existing message.
Long lists show the first 20 dates and an additional-date notice.

Orders and refunds update the original announcement and saved reminders. Moving an
order between dates refreshes both dates, with another reconciliation after five minutes.
Pending purchases reduce the remaining total, including when the organizer limits
the overall event capacity below the total ticket quantities.
An unpublished event is marked **No longer published** and loses its registration
action even if ticket inventory is temporarily unavailable. Republishing restores
the saved message. Private events are not announced.

## Troubleshooting

- **Ticket availability unavailable:** Eventbrite did not provide numeric inventory.
  If only capacity is unknown, the message still shows the sold total alongside
  **Remaining count unavailable**.
- **Old ticket totals:** check the refresh time. Provider updates can take several
  minutes. Ask an administrator to inspect failed Eventbrite work if totals remain old.
- **Missing messages:** check the configured channel and the bot's permission to
  post there. A deleted announcement is not automatically replaced.
- **Channel changed but an old message stayed:** existing messages retain their
  original channel; new messages use the updated setting.

## Operators

Run `bundle exec rake eventbrite:announce_upcoming` for the next 24 hours, or
`bundle exec rake "eventbrite:announce_upcoming[7]"` for seven rolling days.
There is no automatically installed reminder schedule or Portal Jobs button.
The command reports posted, updated, skipped, deferred and failed counts.
Minute recovery retries durable work; see the Rails Eventbrite guide before
repairing failed or ambiguous sends. Never blindly repost an uncertain delivery.
Duplicate notifications preserve retry delays and do not create another initial
announcement. Newly published series may take several minutes to appear while
Eventbrite makes their dates available.

If the command reports failures, read the per-delivery error details. A record with
`previously_failed=true` was already stopped; running the same command again does
not retry it. Correct the reported channel access, token permission or message
validation issue first. Then use `eventbrite:retry_failed` for known failures and
rerun the reminder command. That retry task also resets failed webhook work.
An ambiguous send or a send marker without a message timestamp requires checking
Slack and reconciling the receipt before retrying, to avoid duplicate posts.
Rate limits defer automatically until Slack's retry deadline. A Honeybadger API-key
warning concerns error reporting and does not identify the Slack delivery failure.

The command also shows the configured and effective destination for new posts.
In test mode, all new messages go to `test_channel`, even if **Upcoming Events
Channel** is set to `general` or a channel ID. Confirm that the bot can access
`test_channel`. Real-channel delivery requires `SLACK_ENV=production` on the web
process, workers and tasks; this changes routing for all Slack integrations.
Setting only `RAILS_ENV=production` does not change Slack routing. Keep test and
production receipts separate.

For each new Slack `ChannelNotFound` response, application logs and command stderr
include `[SlackChannelNotFound]`, the API operation, destination mode and actual
channel argument (null, a name or an ID). This covers posts, edits and other Slack
API operations. Existing stopped deliveries produce no new API request; correct
the cause and follow the known-failure retry procedure above.
