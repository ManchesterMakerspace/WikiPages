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
