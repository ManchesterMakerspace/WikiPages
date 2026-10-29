---
title: Member List Indicators
description: "For admins and the board: what the status, email, Slack, Drive and two-factor indicators on the Members list and a member's profile mean."
published: true
date: 2026-10-29T18:00:00.000Z
tags: portal, admin, members
editor: markdown
dateCreated: 2026-10-29T18:00:00.000Z
---

# Member List Indicators

The **Members** list and each member's profile show small indicators. Hover over any of them to see the details. Only admins and the board see the Slack and Drive indicators.

## Membership status

The status shows **Active**, **Expired**, **N/A** (no term yet), **Not started**, **Revoked**, **Inactive**, **Non-Member** or **Suspended**.

A member whose term is running but who has never been issued a key fob shows **Fob not issued** beside the status, with an amber dot while the term is current:

| Member | Shows |
| --- | --- |
| Term running, no fob issued | **Active · Fob not issued** (amber) |
| Term ended, no fob issued | **Expired · Fob not issued** |
| Signed up but no term yet | **N/A** |
| Has a fob | **Active** or **Expired**, as usual |

Issuing the first fob removes **Fob not issued**, and a member who signed up through the portal becomes Active. A **Paid — Not Started** chip beside the status means the member has paid but their term has not started because no fob has been issued. A term staff set by hand, such as a free month from a class, starts when it is set, so check that a fob is issued as well.

## Email

| Icon | Meaning |
| --- | --- |
| Green check | The last email to the member's current address was delivered, opened or clicked. |
| Blue clock | An email was sent but there is no delivery report yet. This normally clears within minutes. |
| Amber warning | A temporary problem, a spam complaint, an unsubscribe, or an email sent more than a day ago with still no report. |
| Red error | The address cannot be reached: the email bounced, was rejected, or sending to it was suspended. |
| Faint envelope | No email has been sent to this address yet. This is normal for long-standing members. |

The tooltip shows the time of the last report and the address. A bounce stays until the member's email address changes. The member's **Email Log** tab lists their last 100 email events.

When an email to a member bounces, the member gets a Slack message if their Slack is linked, and a message is posted to the members relations Slack channel. It is posted once per address, so the channel does not repeat itself.

## Slack and Google Drive

The Slack and Drive indicators show where the member's invitations stand. Green is complete. Amber means waiting, for example for the member to accept the Slack invite or for a fob and future expiration before Drive access can be set up. Red means something needs attention, such as a manual invitation, or provisioning is blocked by the member's status. Grey means an invitation is confirmed but acceptance has not been verified, or nothing has been reconciled yet.

When the Slack indicator is red because a manual step is needed, hover over it. The tooltip says why, for example that the member's email was changed, that Slack rejected the invite because the account that sends invites has not verified its email, or that the member is not eligible because their membership has expired. See [Register a Member](/digital-makerspace/admin/register-member#email-changes) for what to do after an email change.

## Two-factor authentication and role

A green shield means two-factor authentication is on. Grey means it is not. A badge beside the name shows **Admin**, **Board** or **RM** (resource manager). Members have no badge.

*Last reviewed: October 2026*
