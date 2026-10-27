---
title: Audit Log
description: "The portal keeps a record of important changes. Admins and board members can view it."
published: true
date: 2026-10-23T12:00:00.000Z
tags: portal, admin, board
editor: markdown
dateCreated: 2026-10-23T12:00:00.000Z
---

# Audit Log

The portal keeps an audit log: a record of important changes, such as who changed a member, a billing option, a checkout or a portal setting, and when. It is only for admins and board members, who see **Audit Log** in the portal menu. Other members cannot see it.

## Finding entries

Choose **Filters** to narrow the log by **Category**, **Event**, **Changed By**, **Member Affected**, and dates.

- **Category** opens on **All except Slack messages**, so routine bot posts do not bury other changes. Choose **All** to include them, or pick one category: **Email**, **Slack messages**, **Settings & system**, **Members & accounts**, **Billing**, **Rentals**, **Checkouts, tools & shops**, **Reservations**, **Fix tickets** or **Volunteer**. **Other** holds any event that has not been sorted into a category yet.
- **Event** lists only the events that are in the log, narrowed to the category you picked. Choosing a different category clears the Event.

Choose **Show detail** on a row to see what changed.

## Emails and Slack messages

- **Email Sent**: each email the portal sends to a member is recorded, with the member under **Member Affected**.
- **Slack Message Sent** and **Slack Message Failed**: each Slack message the portal posts, to a channel or as a direct message, is recorded from the time this was added. Older messages are not in the log. A direct message shows the member it went to under **Member Affected**, when that member's Slack account is linked. **Show detail** shows the channel, whether Slack accepted the message, the text, and under **After** which part of the portal sent it, Slack's message ID and, for a failure, Slack's reason.

How to read these entries:

- **Sent** means Slack accepted the message. Slack does not tell the portal whether anyone read it.
- **No entry at all** means the portal never tried to send it, for example because the member's Slack account is not linked.
- Not recorded: the private replies that only the person who typed a Slack command can see, and edits to messages that were already posted.

Other pages in this wiki say a change "is recorded in the audit log". This is where to look.

*Last reviewed: October 2026*
