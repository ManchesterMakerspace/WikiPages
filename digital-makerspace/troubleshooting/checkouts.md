---
title: "Troubleshooting: Tool Checkouts"
description: Fixes for common tool checkout problems, for members, approvers, board and admins.
published: true
date: 2026-10-16T01:33:11.499Z
tags: portal, checkout, troubleshooting
editor: markdown
dateCreated: 2026-10-16T01:33:11.499Z
---

# Troubleshooting: Tool Checkouts

Find your situation. Start with the section for your role.

- [Members](#members)
- [Approvers and resource managers](#approvers-and-resource-managers)
- [Board and admins](#board-and-admins)

---

## Members

### "Your membership must first be activated and you must complete your Orientation checkout before requesting this Safety Checkout"

Your membership is not active, or it has expired. Open your profile and check the membership status and expiry date. If it has expired, renew it. If you have just joined, you may still be pending: complete your orientation and key fob steps. A few tools allow pending members to request a checkout; most do not. If your status looks wrong, ask the board.

### "Complete all prerequisite checkouts before requesting this tool"

This tool needs another checkout first (for example a shop orientation). Look at the tool's page for the prerequisites, get checked out on those, then request again.

### "A checkout record already exists for this tool"

You are already checked out on this tool, or you were checked out before and it was later revoked. Check **Tool Checkouts** > **My Checkouts**. If it is not there, ask an approver or the board. A revoked checkout has to be reinstated by an admin or board member before you can be checked out again.

### "An open request already exists for this tool"

You already asked. Look under **My Checkout Requests**. You can edit the note, or delete the request and ask again.

### "No checkout required"

Anyone may use this tool without a checkout. There is nothing to request.

### "Tool unavailable"

The tool or its shop is turned off, hidden or out of service for now. Ask the shop's Resource Manager.

### A tool is missing from the list

The **Available Tools** list leaves out a tool if it needs no checkout, you are already checked out on it, your checkout for it was revoked, or the tool or its shop is hidden. While your membership is still pending, only tools open to pending members are listed.

A tool you cannot request yet is still listed. **Missing Prereq** in the **Status** column means a prerequisite checkout is missing (the **Prerequisites** column names it), and **Request Pending** means you have already asked. If your membership is not active, the list does not load at all and you see the membership message described above.

### My request is taking a long time

Approvers are volunteers, and a request is reminded about in the Resource Managers channel at 5, 10 and 15 days. The quickest route is to message the shop's Slack channel, or ask in person at an open house. After 20 days with no checkout the request closes automatically and you are told, and you can ask again or contact the board.

### I was already checked out in person but the portal does not show it

Ask the approver to record it in the portal using **Check Out Member**. Until they do, the portal does not know.

### My request was declined

Read the reason in the Slack message. Fix whatever it says, then submit a new request.

### I am not getting Slack messages

Check that your Slack account is linked to your membership and that you have not turned off direct notifications. The portal does not email these messages. Slack accounts are matched to members by email address, so check that the email on your Slack profile is the one on your membership. If they differ, ask a board member.

### The QR code on the tool does not work

The code opens the tool's page in your browser. If it fails to load, check your phone's connection and try again. Signing in is required to request a checkout. If a code gives a "not found" page, tell the shop's Resource Manager: the tool may have been removed or hidden.

---

## Approvers and resource managers

### The confirmation screen says the member cannot be checked out

The screen shows the reason, and for missing prerequisites it lists them (**Missing: ...**). The common reasons:

| Message | What it means | What to do |
| --- | --- | --- |
| Membership must be activated / orientation first | Member is expired, inactive, revoked, suspended, or pending on a tool that does not allow pending members | Ask them to renew or complete sign-up; board can fix a wrong status |
| Complete all prerequisite checkouts | A required earlier checkout is missing | Check them out on the prerequisite first |
| A checkout record already exists | They are already checked out here, or an old checkout was revoked | See below |
| Tool unavailable | The tool or shop is disabled | Ask the RM or an admin |

### I scanned a fob and nothing happened, or it found the wrong person

- **iPhone:** phones cannot read fobs in the browser. Use **Search by name or email**.
- **Android:** use Chrome, make sure NFC is on, and hold the fob to the back of the phone. The page must be on the secure (https) site.
- A fob reported **lost or stolen** is refused on purpose. The member needs a replacement fob from the board.
- If the fob is not assigned to anyone, search by name instead and tell the board so the fob can be assigned.
- If it finds the wrong person, do not tap **Check Out**. Tap **Back**, search by name, and tell the board.

### The Tool list is empty in the Check Out box

Choose the **Shop** first. The tool list only shows tools in that shop that you can approve.

### I do not see Check Out Member

You are not an approver for that tool or shop, or you are not signed in. Ask the shop's Resource Manager to add you as an approver (see [Tool groups and approvers](/digital-makerspace/resource-managers/tool-groups-and-approvers)).

### A request is not in my list

Requests from members whose membership has expired, lapsed or been revoked, or who are missing a prerequisite, are hidden until that is fixed. A closed, declined or timed-out request is also gone from the open list.

### A request is still showing though we did the checkout

Use **Check Out Member** to record it. That closes the open request. Until then it stays in reminders.

### I did not get the daily summary

You only get it when there is a new request since your last one, or an open request is exactly 5, 10 or 15 days old. You also need a linked Slack account with direct notifications on. Admins and board members only get it if they are also an RM or approver.

### The checkout shows as Revoked but the member passed again

Check the **Notes** column on the roster first (approvers, Resource Managers, board and admins can see it) for why it was revoked. A row marked *Reinstated* is no longer blocking: the member has a newer active checkout.

The portal does not check someone out again over a revoked record. Tell the board or an admin, who can reinstate it.

---

## Board and admins

### Reinstate someone after a revoked checkout

A revoked checkout stays as a record and blocks a new request or checkout. Admins and board members can lift this from **Tool Checkouts** > **Checkout Roster**: set **Status** to *Revoked only*, tick the row and click **Reinstate Checkout**, then give a reason. The revoked record is kept and a new active checkout is added. The old row then shows a grey *Reinstated* status (filter by **Status** > *Reinstated* to see both rows), and the **Notes** column shows the revocation and reinstatement reasons to approvers, Resource Managers, board and admins only. See [Revoke a checkout](/digital-makerspace/approvers/revoke-a-checkout#reinstate-a-revoked-checkout-admins-and-board).

### A checkout was recorded by mistake

The portal has no delete. Revoking it leaves a revoked record, which blocks a later correct checkout until an admin or board member reinstates it. Prefer telling an admin before revoking.

### Who did what, and when

Open **Audit Log** (admins and board). Checkout events, fob lookups and request declines (including automatic timeouts) are recorded there with who and when.

### Reminders are not appearing in the Resource Managers channel

Open **Portal Settings** and check the **Slack** tab: the Resource Managers channel must be set. Also check the **Jobs** tab to see that the checkout request reminder and digest jobs have run.

### Slash commands say a shop is not configured

The shop's **Slack Channel** must be filled in under **Tool Checkouts** > **Shops**. It is also how `/checkout` and `/reserve` find the shop.

### The Checkout Required sign has a blank footer

The shop has no Slack channel set. Set it on the shop, then download the sheet again.

### A QR code or sign gives an error

The sign's QR code is a permanent short link. Short links cannot be created if the site's public address is not configured or the database is unreachable; this is a server-side problem and belongs on the restricted operations page.

### Approvers cannot see or approve requests

Open **Tool Checkouts** > **Approvers** and tick their row and use the edit button to check their scope. Approval for a group needs a shop assignment or a group assignment, not just individual tools in the group.

## Checkout expired or reservation ends after expiration

A checkout is valid through its displayed date in Eastern time. Missing dates
mean Never expires. Select **Expired** in your checkout list and use
**Request renewal** when available, then complete any required training and wait
for approval. If the checkout was revoked, contact an admin or board member.

Reservation errors name checkouts that expire before the reservation ends,
including shop and group prerequisites. Request renewal or choose an earlier
end time. An end exactly at midnight after the expiration date is permitted.
Existing bookings are not automatically canceled after expiration edits, but
editing a booking rechecks its prerequisites. Cancellation remains available.

## Checkout operations remain busy after a bulk expiration update

A bulk update keeps the shop locked until its transaction finishes. If its
worker crashes, ask an administrator to confirm the worker has stopped and
recover the orphan catalog lock using the Rails jobs/services runbook. Do not
clear a lock while an update may still be running. Failed transactions do not
leave partially updated expiration dates or audits.
