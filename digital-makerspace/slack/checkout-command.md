---
title: The /checkout Slack Command
description: Request and approve tool checkouts with the /checkout Slack command.
published: true
date: 2026-10-16T01:33:11.499Z
tags: slack, checkout, portal
editor: markdown
dateCreated: 2026-10-16T01:33:11.499Z
---

# The /checkout Slack Command

You can request and approve tool checkouts without opening the portal. Menus, lists and help are shown only to you. Requests and approvals post the same messages and channel announcements the portal does.

## Before you start

Your Slack account must be linked to your portal membership. If it is not, Slack replies *Link your Slack account to a Member Portal account before using /checkout.* Accounts are matched by the email address on your membership, so make sure it is the same one you use in Slack, or ask a board member to help.

Your membership status decides what you can do. If something is wrong, the command tells you:

| You see | What it means |
| --- | --- |
| *Your membership has expired. Renew it before using checkouts.* | Renew your membership in the portal |
| *Your membership is inactive. Activate it before using checkouts.* | Your membership needs activating |
| *Your membership is suspended. Contact the makerspace before using checkouts.* | Contact the board |
| *Your membership is revoked. Contact the makerspace before using checkouts.* | Contact the board |
| *Your membership is not eligible for checkouts. Contact the makerspace.* | Contact the board |

**Pending** members can use the command, but they can only act on tools that allow pending members.

## The menu

Type `/checkout` on its own to open a menu with four choices, the same for members and approvers:

- **View my checkouts**
- **Request a checkout**
- **Volunteer to do checkouts**
- **View open requests**

If you type it **in a shop's channel**, the menu is for that shop. Anywhere else, it first asks you to choose a shop. A menu works on one shop at a time, so close it and run the command again to switch.

## Commands for members

| Command | What it does |
| --- | --- |
| `/checkout request` | In a shop channel, opens a box with only the tools you can request. Elsewhere, lists your open requests across shops |
| `/checkout request tool-name` | Requests that tool, in the shop whose channel you are in |
| `/checkout active` or `/checkout list` | Lists your active checkouts in this shop |
| `/checkout active all` | Lists your active checkouts in every shop |
| `/checkout volunteer` | Ask to become a checkout approver for a tool you are checked out on |
| `/checkout help` | Shows the commands available to you |

Request commands must start in a **shop's own Slack channel**. If the channel is not set up as a shop, Slack replies *No shop is configured for #(channel). Run /checkout request from a shop channel.*

Your own open requests also appear under **View open requests**. Open one to edit its note or cancel it. Only you can edit or cancel your own request.

## Commands for approvers

| Command | What it does |
| --- | --- |
| `/checkout @member tool-name` | Checks the mentioned member out on that tool. You can use the member's portal email address instead of a mention |
| `/checkout @member group-name` | For a tool group, opens a review box first, with the message *Review the group checkout before approving.* |
| `/checkout` > **View open requests** | The same open requests you see in the portal. You can approve or decline from here |

Run `/checkout @member tool-name` **in the shop's own channel**. If you do not, Slack explains: *Checkout approvals and new requests must start in the appropriate shop channel*, and lists the shop channels to join.

After you send it you see *Processing checkout of (tool) for (member)...* and then *Checkout approved: (tool) for (member).*

Things that can go wrong, with the message you will see:

| Message | What to do |
| --- | --- |
| *You are not authorized to check out members on tools.* | You are not an approver for that tool. Ask the shop's Resource Manager |
| *Use /checkout @member tool-name* | The command was missing the member or the tool name |
| *No shop is configured for this channel.* | Run it in the shop's channel, or ask an admin to set the shop's Slack channel |
| *Tool not found in this shop.* | Check the tool's exact name, or that you are in the right shop channel |
| *No member found. Try their Member Portal email address.* | Use the email address instead of the mention |
| *A checkout record already exists for this tool* or another eligibility message | The member cannot be checked out on that tool. See [Troubleshooting: checkouts](/digital-makerspace/troubleshooting/checkouts) |
| *The checkout could not be completed. Check the Member Portal before trying again.* | Look in the Member Portal to see whether it was recorded before trying again |

## Becoming an approver

If you are checked out on a tool and know it well, run `/checkout volunteer` and choose the tool, with an optional note. The shop's Resource Managers are messaged with your note, your checkout date and your join date. A Resource Manager approves or declines, and you are told the result. Approval makes you an approver for that tool only.

## Things to know

- **The portal is always there as a fallback.** See [Request a checkout](/digital-makerspace/members/request-a-checkout) and [Check out a member](/digital-makerspace/approvers/check-out-a-member).
- **Long tool lists.** Slack can only show 100 tools in a picker. If more are available, the command tells you to use the portal.
- **Help.** `/checkout help` shows only the commands you can use. The approval command is listed only for admins, board members, Resource Managers and assigned approvers.

## Related commands

Reservations use `/reserve` and volunteer tasks use `/volunteer`. They will have their own pages.

## Training plans and expired checkouts

Checkout request creation, your request details, and your checkout details show
a clickable **Checkout training plan** link when configured. **View my checkouts**
also includes expired checkouts and labels their expiration date. Expiration
does not expose private tool notes through the old checkout. Use the Member
Portal’s Expired filter and **Request renewal** to request another approval.
