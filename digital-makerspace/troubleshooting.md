---
title: Troubleshooting
description: Why didn't that work? Quick answers for members about logging in, payments, key fobs, invitations, checkouts and rentals.
published: true
date: 2026-10-29T18:00:00.000Z
tags: troubleshooting, members, help
editor: markdown
dateCreated: 2020-01-22T13:33:00.704Z
---

# Troubleshooting

Something did not happen the way you expected? Find your situation below. If you cannot fix it yourself, ask in **#discuss-talk-to-the-board** on Slack, or come to an open house.

## Signing in

### I cannot sign in, or I forgot my password

On the sign-in page choose **Forgot your password?**, enter the email address on your membership, and submit. Check your spam folder, because the email comes from the makerspace. The link in the email works for 24 hours. If it has expired, request a new one. You can also sign in with a connected Google, Apple, GitHub or Microsoft account if you set one up. See [Log In](/digital-makerspace/log-in).

### I never set a password

If a board member or admin created your account, it has no password yet. Use **Forgot your password?** to set one.

### The email address is wrong, or I changed it

You can change the email on your profile, or ask a board member to correct it. Please also change your email in Slack at the same time, in Slack's account settings. Slack sends a confirmation to the new address. Tell the board you did it. That keeps the same Slack account instead of creating a new one.

Your Google Drive access moves to the new address automatically. If you do not change your email in Slack, a board member has to send a new Slack invitation to the new address, which deactivates your old Slack account. Accept the new invitation from your email.

## Your membership and key fob

### I paid, but my membership is not active

Your membership time starts when you receive your key fob, not when you pay, and you do not lose any time while you wait. Come to an open house for your orientation and fob, or ask in #discuss-talk-to-the-board. If a long time passes between paying and getting your fob, your billing date and your expiration date will not match. That is normal.

### My key fob does not open the door

A fob works only while your membership is active and not expired, and only if it is registered to you. Check your expiration date on the portal's **Home** page. A fob that was reported lost or stolen is turned off on purpose. Ask the board or come to an open house for a replacement.

### My expiration date looks wrong

Look at **Subscriptions** in the portal menu. If you pay by subscription, the date moves forward after each successful payment. If something does not look right, tell the board.

## Payments

### My payment failed

You should get an email, and a Slack message if your Slack account is linked. The message includes the reason. Open **Payment Methods** in the portal menu to add a new card or change the one on file, then pay what is due from the **Dues** tab on your profile. A failed subscription payment is also tried again automatically. See [Making Payments](/digital-makerspace/payments).

### I was charged and I think it was a mistake

Refunds are generally not given. See [Payment History and Refunds](/digital-makerspace/refunds) for what to do.

### I do not want to renew

Cancel your subscription before the renewal date. See [Manage Membership](/digital-makerspace/manage-membership).

## Invitations and messages

### I never got my Slack or Google Drive invitation

Your Slack invitation is sent once your membership is active. The Google Drive invitation also needs your key fob to be registered. Both can take a little while after you join, because they are sent in batches. Check your spam folder, and make sure you are checking the email address on your membership. If it still has not arrived, ask in #discuss-talk-to-the-board.

### I am not getting emails or Slack messages

Check your spam folder first. Billing and rental messages are always sent. If you unsubscribed from makerspace emails, you will still get these. Messages in Slack only reach you if your Slack account is linked to your membership. Slack accounts are matched to members by email address.

If an email to you could not be delivered, for example because the address has a typo or the mailbox no longer exists, and your Slack account is linked, you get a Slack message saying so. The board is told as well. Update the email address on your profile, or ask a board member to correct it.

## Tools

### I cannot request a checkout, or my request has not been approved

See [Troubleshooting: Tool Checkouts](/digital-makerspace/troubleshooting/checkouts). It explains every message you can see and what to do.

## Reservation announcements

### The Reserve button in a Slack summary will not open a form

You need a linked, active, unexpired Member Portal account. Read the private **Reservation unavailable** message, sign in to the portal and check your membership. The shop may be hidden, out of service, or have no resources you can reserve. Ask its Resource Manager or use **Reservations** in the portal. The button does not bypass required tool checkouts.

### An empty-shop invitation is missing or changed

The shop's **Announce empty reservation agendas in Slack** option starts off. Ask its Resource Manager about enabling it. Invitations appear only when the channel's whole day is empty; bookings from yesterday, blackouts and unavailable resources can prevent them. A booking or setting change can replace an invitation in the same message. **No reservations to announce for [date]** is a neutral update, not a promise that every resource is available. If a linked live agenda still shows an edited or cancelled overnight booking, an admin can use **Portal Settings → Jobs → Daily Reservation Announcements → Run Now** after 7 AM Eastern to refresh it. This also works for shops with only a tool Users Channel; the summary itself may stay unchanged.

### Yesterday's empty message disappeared

The portal tries to remove yesterday's empty invitation or neutral empty summary before posting today's message in that channel. Nonempty summaries stay. Cleanup can fail without stopping today's post; an admin can check the job logs.

### A summary or its agenda link looks stale

Check the date printed in the summary. **Live today agenda** links always open the current rolling canvas, including from yesterday's message. Deleting the last shop represented in today's summary removes the message instead of leaving a reservation button for a deleted shop; Slack deletion failures are retried. Deleting or moving a tool, or changing its Users Channel, refreshes the old and new destinations; abandoned summaries are removed and shared summaries retain their other resources. Failed channel lookups preserve the existing message until Slack can resolve the configuration. Ask an admin to check **Portal Settings → Jobs → Daily Reservation Announcements** and use **Run Now** after 7 AM Eastern. Slack channel or canvas-access problems may need the admin's attention.

## Storage rentals

### I cannot rent a space

You need an active membership and no past-due invoices. See [Rent a Storage Space](/digital-makerspace/members/rent-a-space), which has a table of the messages you may see.

## Volunteering

### My volunteer work does not show yet

Points are added after the work is reviewed. If you completed a task, mark it complete in the **Volunteer** tab on your profile, then ask in #discuss-talk-to-the-board if it has not been recognized after a few days.

## The portal itself

### A page will not load, or something looks wrong

Use the **Retry** button if you see one. If the page is still broken, sign out and back in, then try another browser. If it keeps happening, tell the board what you were doing and what you saw, and include the time.

### I cannot find something in the menu

Some menu items depend on your role. See [The Member Portal Home Page and Menu](/digital-makerspace/members/home-and-navigation).

*Last reviewed: October 2026*
