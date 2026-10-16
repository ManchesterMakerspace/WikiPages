---
title: Request a Tool Checkout
description: How members request a tool checkout, by QR code or through the member portal.
published: true
date: 2026-10-16T01:33:11.499Z
tags: portal, checkout, members
editor: markdown
dateCreated: 2026-10-16T01:33:11.499Z
---

# Request a Tool Checkout

Some tools are marked **Checkout Required**. A checkout is a hands-on safety session with a trained volunteer (an *approver*) so you can use the tool without hurting yourself, others, or the tool. Depending on the tool it can take anywhere from 15 or 30 minutes to a few hours. Each shop's Resource Manager decides what the checkout involves.

You must be checked out on a tool before you use it. Most checkouts are quick, but some tools need a longer class, which may have a cost. The shop's page on this wiki or its Slack channel will tell you what to expect for a particular tool.

## Before you start

You can request a checkout when all of these are true:

- You have an **active membership** that has not expired.
- You have completed any **prerequisite checkouts** for that tool (for example, a shop's orientation checkout).
- You do not already have a checkout for that tool, and you do not already have an open request for it.
- The tool and its shop are available (not disabled or hidden).

The tool list in the portal only shows tools you can request right now, so if a tool is missing, see [Troubleshooting: checkouts](/digital-makerspace/troubleshooting/checkouts).

## Ask for a checkout

### Option 1. Scan the QR code on the tool

1. On your phone, scan the **Checkout Required** sign on the tool.
2. On the tool's page, tap **Request checkout**.
3. Sign in to the member portal if you are asked to. You land on a page titled **Request checkout** showing the tool.
4. If you cannot request this tool yet, a blue message explains why (for example, a prerequisite checkout is missing). Otherwise tap **Request checkout**. A box titled *Request Checkout: (tool name)* opens.
5. Optionally, add a **Note** for the approvers (up to 128 characters), for example when you are free.
6. Tap **Submit Request**. You will see *Checkout request submitted.*

### Option 2. In the member portal

1. Sign in at members.manchestermakerspace.org and open **Tool Checkouts** from the menu. You will see the tabs **My Checkouts**, **Requests** and **Shop Map**.
2. Open the **Requests** tab. Under **Available Tools**, use the **Shop** selector (it starts on *All shops*) or the search box to find the tool.
3. Check the **Prerequisites** column. If you have what you need, the **Status** column shows a blue **Send Request** button. Click it. (If a prerequisite is missing it says **Missing Prereq**, and if you have already asked it says **Request Pending**.)
4. A box titled **Request Tool Checkout** opens, naming the tool and shop. Optionally add a **Note** for the approvers (up to 128 characters), then click **Submit Request**.
5. Your request now appears under **Open Requests** on the same tab.

### Option 3. In Slack

Use `/checkout request`. See [the /checkout command](/digital-makerspace/slack/checkout-command).

## What happens next

1. **The shop is told.** If the tool announces requests, a message appears in the tool's channel. If your Slack account is linked to your membership, you also get a Slack message confirming the request, and your shop may add its own note to it.
2. **Approvers see it in their daily summary** and arrange a time with you. They may also contact you directly. The fastest way to get a checkout is to message the shop's channel, or ask in person at an open house.
3. **If nothing happens, we nudge.** An open request is reminded about in the Resource Managers channel at 5, 10 and 15 days.
4. **After 20 days with no checkout, the request is closed automatically** and you are told by Slack message. You can contact the board on Slack or visit an open house, or just submit a new request.

You can **edit the note** or **delete** your request any time before it is closed: select it under **Open Requests** and use **Edit Note** or **Delete**.

### When you are checked out

You get a Slack message naming the tool, the shop and the approver, plus any private notes for the tool (such as a lock combination). If the tool has a users channel, you are added to it. The tool now shows under **My Checkouts**.

### If the request is declined

You get a Slack message with the approver's reason. A decline does not block you: once the issue is fixed you can submit a new request for the same tool.

> If you were already checked out in person, an approver records it in the portal and your request closes by itself.
{.is-info}

## Check what you are checked out on

Open **Tool Checkouts** > **My Checkouts**. It is titled **My Active Tool Checkouts** and lists everything you are checked out on. Use **Filter by Shop** to narrow it down. In Slack, `/checkout active` lists your active checkouts in the current shop channel, and `/checkout active all` lists them across shops.

## Need help?

See [Troubleshooting: checkouts](/digital-makerspace/troubleshooting/checkouts).
