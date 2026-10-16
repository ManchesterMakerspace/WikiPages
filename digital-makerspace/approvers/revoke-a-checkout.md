---
title: Revoke a Checkout and Review the Checkout Roster
description: 
published: true
date: 2026-10-16T01:49:30.260Z
tags: portal, checkout, approvers, resource-managers
editor: markdown
dateCreated: 2026-10-16T01:49:30.260Z
---


# Revoke a Checkout and Review the Checkout Roster

The **Checkout Roster** lists the checkouts you are allowed to see: who is checked out on what, when, and by whom. Use it to answer "is this member checked out?", and to revoke a checkout when someone should no longer use a tool.

You only see checkouts for the tools you can approve. An approver assigned to one tool sees only that tool's checkouts, while a shop's Resource Manager sees the whole shop, and admins and board members see everything.

## Find a checkout

1. Open **Tool Checkouts** > **Checkout Roster**. Approvers and Resource Managers land on this tab by default.
2. Narrow the list with the filters at the top:
   - **Filter by Shop**: choose a shop, or leave it on *All Shops*.
   - **Filter by Tool**: shows *Select a shop first* until you pick a shop. Then it offers *All Tools in Shop* and each tool.
   - **Status**: *Active only* (the default), *Revoked only* or *All*.
   - **Include expired, revoked and inactive members**: unticked by default, so people whose membership has lapsed do not clutter the list. Tick it when you need to see them.
3. Use the **Search** box above the table to find someone by name.

Each row shows the **Member** (name and email), the **Tool** and its shop, **Checked Out** (the date, and how it was signed off, for example *via portal*), **Approved By**, and **Status**: a green *Active* or a red *Revoked*.

## Revoke a checkout

1. Tick the box on the member's row. A **Revoke Checkout** button appears next to **Check Out Member**.
2. Click **Revoke Checkout**. A box opens: *Revoke (member)'s checkout for (tool) in (shop)?* It reminds you that *the member will be notified via Slack DM* and that *the reason is internal only*.
3. Type the **Reason for revocation (internal)**. It is required.
4. Click **Revoke**. Click **Cancel** to close the box without revoking.

The row leaves the *Active only* list. To see it again, set **Status** to *Revoked only*. It shows with a red **Revoked** status.

### What happens when you revoke

- The member receives a Slack message naming the tool and shop. It does **not** include your reason.
- They are removed from the tool's users channel, if it has one.
- The tool no longer appears under their **My Checkouts**, and it disappears from their **Available Tools** list, so they cannot ask for it again.
- If someone other than the original approver revokes it, the original approver is told, as long as they are still allowed to approve that tool.
- If the member was an approver for that tool, that assignment is removed.
- If the original approver earned the automatic volunteer credit for the checkout, the credit is reversed.
- The checkout stays in the roster as **Revoked**, so there is a permanent record.

> **A revoked checkout still blocks a new one.** The portal will not check the same member out on that tool again, and the member cannot request it. If someone who was revoked has retaken the safety session and should be reinstated, tell the board or an admin. [confirm the agreed process]
{.is-warning}

## When not to revoke

- **You recorded the wrong member or tool by mistake.** Tell the board or an admin rather than revoking, because revoking leaves a permanent revoked record that blocks the correct checkout. [confirm process]
- **Membership has lapsed.** You do not need to revoke. Lapsed members are hidden from the roster by default, and their checkouts are still there if they renew.

## See also

- [Check out a member](/digital-makerspace/approvers/check-out-a-member)
- [Troubleshooting: checkouts](/digital-makerspace/troubleshooting/checkouts)
