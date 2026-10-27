---
title: Reservation Checkout Expiration in Slack
description: How /reserve handles a required checkout that expires before your reservation ends.
published: true
date: 2026-10-27T12:00:00.000Z
tags: portal, slack, reservations
editor: markdown
dateCreated: 2026-10-27T12:00:00.000Z
---

# Reservation Checkout Expiration in Slack

When you reserve with **/reserve**, every checkout the tools require must still be valid for the whole reservation, through the **calculated end** the form shows. Changing the **Date**, **Start time** or **Duration** refreshes the choices and any warning.

- **Durations stop where a checkout expires.** A checkout is valid through its displayed date (Eastern time), so a reservation can run until midnight at the start of the next day. Whole-day bookings follow calendar days.
- **Duration too long?** The form shortens it to the longest duration that works.
- **Nothing fits?** The form shows **Review selection** instead of **Reserve** and names the checkout that is the problem. Choose an earlier date or start time, change the tools, or ask for a renewal in the member portal. See [Request a Tool Checkout](/digital-makerspace/members/request-a-checkout).
- **Tools you can't reserve through that time are hidden** unless you already selected them. A selected tool marked **(checkout required)** stays visible so you can fix it. Shop and group prerequisites apply too.

Check the calculated end before you submit. A checkout that expires later does not change a reservation you already made. For the rest of the steps, see [Reserve a Shop or Tool](/digital-makerspace/members/reserve-a-shop-or-tool).

*Last reviewed: October 2026*
