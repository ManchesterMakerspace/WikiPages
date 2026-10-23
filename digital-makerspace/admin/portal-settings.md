---
title: Portal Settings
description: "For admins: what each tab of Portal Settings controls, including Slack channels, volunteer settings, scheduled jobs, two-factor enforcement and document templates."
published: true
date: 2026-10-23T12:00:00.000Z
tags: portal, admin, settings
editor: markdown
dateCreated: 2026-10-23T12:00:00.000Z
---

# Portal Settings

Portal Settings is where admins set up how the portal behaves behind the scenes. Open **Portal Settings** from the portal menu. Only admins see it. Changes take effect immediately, so check a value before you save it.

The page has six tabs: **Slack**, **Volunteer**, **Reservations**, **Jobs**, **Security** and **Templates**.

To change a text value, choose the pencil beside it, type the new value and choose the save (disk) icon. The cancel (x) icon discards the edit. Switches save as soon as you flip them. Never paste a token or other secret value into a page, message or ticket.

## Slack

- **Slack Channels:** the channel names, without the `#`, that the portal posts to.
  - **Treasurer Channel:** billing alerts and discount notices.
  - **RM Channel:** Resource Manager notices, such as checkout requests and reminders. The default is `resource_managers`.
  - **Members Relations Channel:** membership and volunteer approval alerts, and payment announcements. The default is `members_relations`.
  - **Logs Channel:** system logs and alerts about Slack users who are not linked to a member.
  - **New Members Channel:** welcome messages for new Slack members.
  - **Fix Tickets Channel:** where new and updated repair tickets are announced. Saving it blank turns announcements off.
  - **Volunteer Pending Channel:** notified when a volunteer task is waiting for review.
- **Slack Channel Cache:** shows how many public channels are cached and when the cache last updated. **Clear and Rebuild Cache** refreshes it. Use it if a new channel is not being found.
- **Slack User Sync:** **Enable Scheduled Sync** and **Enable Scheduled Profile Sync** are switches. **Run Now** matches the Slack workspace's users to members by email, which is useful after onboarding a batch of new members. **Resolve Slack Conflicts** opens the screen for members whose Slack account does not match.

## Volunteer

Some labels here still say "credit". Read it as volunteer points.

- **Credits Per Discount**, **Max Discounts Per Year** and **Volunteer Discount** control how points turn into a billing discount. Changing the discount posts a notice to Slack.
- **Rolling Days Counter** and **Leaderboard Top N** control the volunteer displays.
- **Max Credit Per Task** and **Max Credits for Ticket Bounties** cap the points on bounty tasks. The ticket limit is at least 0.5 and changes are recorded in the [audit log](/digital-makerspace/admin/audit-log).
- **Public Bounty Board:** **Require Token** and **Token Value** protect the public bounty page with a token in the address.

## Reservations

**Reservation Token** protects the public 24-hour shop and tool agenda. If you leave it blank, the agenda is public.

## Jobs

Heroku Scheduler cannot run monthly, so a few jobs run every day and only do their work on the day of the month set here: **Slack Channel Cache refresh day**, **Card Expiration Check day** and **Garbage Collector day** (1 to 31).

Below that, each background job shows what it does, when it last ran and whether it **Succeeded** or **Failed**. **Run Now** runs it straight away, whatever the schedule says. Examples are the database backup, the member and invoice reviews, the card expiration check, the reservation canvas rebuild, and the checkout request reminders and digest. A message under the button confirms that the job was queued.

## Security

- **Two-Factor Authentication Enforcement:** switches to require two-factor sign-in for admins, board members and Resource Managers. When required, a privileged member who has not enrolled is sent to their Security settings after login and cannot use the portal until they enroll. All members may turn on two-factor themselves. See [Log In](/digital-makerspace/log-in).
- **Open ticket limit** for repair tickets also appears here.
- **Lock Out New Signups:** sends new visitors to a maintenance page instead of the sign-up form and rejects new registrations. Members who are already part-way through signing up are not affected. Turn it off again when you are done.

## Templates

Documents such as agreements are kept as Google documents and cached by the portal. Each template shows its status: **Cached**, **Not cached**, **Empty document**, **Using embedded template**, **Permission denied** or **Invalid template**.

- **Refresh** fetches the document again. If a refresh fails, the portal keeps using the last good copy.
- **Edit** opens the document in Google.
- **Populate** fills an empty document with the default text.
- **Restore default** replaces the document's content with the built-in default. It asks you to confirm because it wipes out your changes.

Hover over a template to see its placeholders and what to fix when it has a problem.

## Troubleshooting

| Problem | What to check |
| --- | --- |
| Messages are not arriving in a Slack channel | The channel name on the **Slack** tab must match the real channel, without the `#`, and the channel must exist. |
| A new Slack channel is not found | Choose **Clear and Rebuild Cache** on the **Slack** tab. |
| A job does not seem to run | Look at its last run and status on the **Jobs** tab. Use **Run Now** and read the message. |
| A template shows **Permission denied** | Share the Google document with the portal's service account, then choose **Refresh**. |
| A privileged member is stuck on the Security screen | Two-factor is required for their role. They need to finish enrolling. |

*Last reviewed: October 2026*
