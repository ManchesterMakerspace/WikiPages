---
title: Earned Memberships
description: How admins and board members set up and manage earned memberships, which members keep by doing agreed activities instead of paying.
published: true
date: 2026-10-22T12:00:00.000Z
tags: portal, admin, earned-memberships, board
editor: markdown
dateCreated: 2026-10-22T12:00:00.000Z
---

# Earned Memberships

An earned membership is a membership a member keeps up by doing agreed activities, such as helping in the shops, instead of paying. Admins and board members set them up and record the work by hand. Nothing is counted automatically. A member can have only one earned membership, and a member on a paid subscription must cancel it first.

Open **Earned Memberships** from the portal menu. Only admins and board members see it.

## The list

The **Earned Memberships** page lists each earned member with their **Name**, **Expiration** date and **Earned Membership Status** (**Active** or **Suspended**). Tick a row to use **Edit Membership** or **Suspend Membership**. **Create New Membership** is always available.

## Create an earned membership

1. Choose **Create New Membership**.
2. Under **Select a member**, search by name or email and pick the member.
3. Fill in the first requirement:
   - **Requirement Name:** pick a name from the list, or choose **Other** and type your own.
   - **Term Length:** how long one term lasts, from 1 to 12 months.
   - **Count required for completion:** how many times the activity must be done in a term, from 1 to 10.
   - **Rollover Limit:** how many extra completed activities carry into the next term. Leave it blank for no limit (recommended).
   - **Strict reporting?:** makes the person reporting enter the name of each person they helped. This is not recommended.
4. Choose **Add Requirement** to add more. A membership needs at least one.
5. Choose **Submit**.

The member's expiration date is set to the end of the shortest term when you create it. A member on a subscription cannot be given an earned membership, and the page tells you to cancel the subscription first.

## Record activity

Each time a member completes a requirement, someone records it.

1. Open the member's profile.
2. Open the **Membership** tab. It lists the member's reports.
3. Choose **Submit new report** and fill in what was done and how many times.

When the count for a requirement reaches its target, that term is complete and the next one starts. Extra completed activities carry over up to the rollover limit. When every requirement is complete, the member's expiration date moves to the end of the shortest term, and a message is posted in the members relations Slack channel. If a member falls behind, the next term starts from today. You cannot report activity for a future term.

## Change or suspend one

- **Edit Membership** changes the requirements.
- **Suspend Membership** stops the earned membership without deleting its history. Use it when a member switches to a paid subscription. A suspended membership cannot record new reports. It can be reactivated later, but not while the member is on a subscription.

Members with an earned membership do not get the automatic membership expiry reminder emails that subscription-free members get.

## Troubleshooting

| Problem | What to check |
| --- | --- |
| The member cannot be chosen | They already have an earned membership, or they are on a subscription. Cancel it first. |
| The expiration date did not move | The member has not completed every requirement for the current term. Check the reports on their Membership tab. |
| A report is rejected | It may be for a future term, or the earned membership is suspended. |
| You cannot reactivate | The member is on a paid subscription. |

*Last reviewed: October 2026*
