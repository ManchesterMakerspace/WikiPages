---
title: Checkout Expiration
description: Checkout expiration and renewal
published: true
date: 2026-10-19T17:39:40.305Z
tags: portal, checkout, troubleshooting
editor: markdown
dateCreated: 2026-10-19T17:39:40.305Z
---

# Checkout expiration notices

Admins can open Member Portal Settings → Jobs and set **Checkout expiration
advance notice (days)** to a whole number of at least 4 (default 14).
Under **Checkout Expiration Notices**, select **Run Now** to send due messages.
Check the job status afterward. There is no automatic schedule for this job.
Operators can run the same job with `bundle exec rake checkout_expiration_notice`.


Warnings become due at the configured lead time and at 3 days before expiration.
A final notice becomes due after the displayed Eastern expiration date. A late
run sends the most urgent applicable stage only. Each member gets grouped
upcoming warnings and a separate group of newly expired checkouts, by email and
Slack DM where linked. Messages include tool/shop, date, training plan if set,
and a Member Portal renewal link.

Only active unexpired members and pending members eligible for the tool receive
notices. Revoked/suspended members are excluded. Secondary household members
receive their own email. Missing Slack linkage does not block email.

A failed job can be rerun: recorded successful channels are not repeated, and
other members continue after a delivery failure. If a provider accepted a
message but its acknowledgment was lost, retry can duplicate that message.
Changing a checkout date starts a new notice cycle; assigning the same date does
not. Setting Never removes the checkout from future expiry notice runs.