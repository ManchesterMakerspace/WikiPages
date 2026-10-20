---
title: Rental Management
description: How admins, board members and resource managers manage rentals, rental requests, rental spots and rental types, and print rental labels.
published: true
date: 2026-10-20T12:00:00.000Z
tags: portal, rentals, admin, board
editor: markdown
dateCreated: 2019-09-26T12:03:03.898Z
---

# Rental Management

Members rent storage spaces (totes, shelves and similar) themselves in the portal, so most of your work is setting up the spaces, approving the few that need it, and fixing problems. This page covers the **Rental Management** screen. For what members see, read [Rent a Storage Space](/digital-makerspace/members/rent-a-space).

Admins, board members and Resource Managers can manage rentals. Deleting is limited to admins and board members. Open the portal menu and choose **Rentals** under the admin items to reach **Rental Management**. It has four tabs: **Current Rentals**, **Rental Requests**, **Rental Spots** and **Rental Types**.

## How the pieces fit

- A **rental type** is a kind of space, such as a storage tote or a shelf. Each type points at a **billing plan** (an invoice option) that decides the cost.
- A **rental spot** is one physical space with its own number, for example `LR-Tote-1`. It has a type, a location, and a setting for whether it needs approval.
- A **rental** is a member renting a spot. It is created when the member (or you) claims a spot.

Members see prices in the portal, taken from each type's billing plan. Set the cost by choosing the right billing plan on the type, not on the spot.

## Current Rentals

The table lists every rental with its number, description, expiration date, member and status. Use the search box above the table to find one.

Tick a row to enable **Edit Rental**, **Renew** and **Cancel Rental**.

![Current Rentals](/images/rentals/admin-current-rentals.png){width=700px}

### Create a rental for a member

Use this when a member rents on paper or in person, or you need to set one up for them.

1. Click **Create New Rental**.
2. Search for the member by name or email.
3. Under **Select a Rental Spot**, pick the spot. You can pick any spot, even one that is not available.
4. Add **Notes** if useful. Tick **Rental agreement has been signed (paper or verbal confirmation)** only if the member has signed on paper. If you leave it unticked, the member will be asked to sign the agreement.
5. Click **Create Rental**.

The rental is created as **Active**, and an invoice is generated for the member from the spot's billing plan. The member gets a Slack message (if linked) and an email telling them the rental is not valid until the invoice is paid, so they still need to pay it in their **Dues** tab. If the spot's type has no billing plan, no invoice is created.

### Edit, renew or cancel

- **Edit Rental** changes the number, description, expiration, member, notes, and whether the agreement is signed.
- **Renew** extends the rental's expiration. Choose a term of 1, 3, 6 or 12 months and submit. A message is sent to the members relations Slack channel.
- **Cancel Rental** cancels the member's Braintree subscription and sets the rental to cancelled immediately. It cannot be undone, and the dialog repeats the member, number and description so you can check you have the right one.

If a member asks you to end a rental, the member can also do this themselves (**Cancel Rental** on their profile Rentals tab). If they choose to keep it until the end of the paid period, it shows as **Vacating**, and you can use **Mark Vacated** on their Rentals tab once the space is empty.

![Create New Rental](/images/rentals/admin-create-rental.png){width=700px}

![Renew Rental](/images/rentals/admin-renew.png){width=700px}

![Cancel Rental](/images/rentals/admin-cancel.png){width=700px}

## Rental Requests

Requests for spots marked **Requires Admin Approval** wait here. When a member submits one:

- A message is posted in the **Members Relations Channel** (set in Portal Settings, default `members_relations`) with a link to this tab.
- An email goes to the makerspace contact address.
- The member gets a confirmation by Slack (if linked) and email.

Tick a request to see the member, spot and the member's notes, then:

- **Approve**: *Approving will activate the rental and generate an invoice for the member.* The member is notified and then signs the rental agreement and pays.
- **Deny**: you can add a reason, which is sent to the member. The spot becomes available again.

![Rental Requests](/images/rentals/admin-requests.png){width=700px}

![Approve a rental request](/images/rentals/admin-approve.png){width=700px}

## Rental Spots

This tab lists every spot with its location, type, billing plan, whether it needs approval, whether it is currently available, and whether it is active (visible to members).

Tick a spot to use **Copy Link**, **QR Code**, **Label**, **Edit** and **Delete**. **Add Spot** is always available.

![Rental Spots](/images/rentals/admin-spots.png){width=700px}

### Add or edit a spot

Click **Add Spot** (or tick a spot and click **Edit**).

| Field | What it does |
| --- | --- |
| **Spot Number** (required) | The spot's identifier, used in its link and on its label. Letters, numbers, hyphens and underscores only, no spaces, for example `LR-Tote-1`. Must be unique. The form explains problems as you type. |
| **Location** (required) | Where the spot is, for example the room or area. |
| **Rental Type** (required) | Its type, which also sets the billing plan. |
| **Parent Spot Number** | Only for sub-spots, for example `Shelf-1` for `Shelf-1a` and `Shelf-1b`. Leave blank for an ordinary spot. |
| **Description** | Shown to members. |
| **Notes** | Private notes. |
| **Requires Admin Approval** | Tick for spots the board must approve before the member can rent. Unticked spots are self-service. |
| **Active (visible to members)** | Untick to hide a spot from members without deleting it. |

![Add Rental Spot](/images/rentals/admin-add-spot.png){width=700px}

### Print a label, or copy the QR code

Every spot should carry a label with a QR code, so members can rent it from their phone.

1. Tick the spot and click **Label**.
2. Choose the **Label size**: **4″ × 6″ (portrait)** or **3½″ × 1⅛″ (address label)**.
3. Click **Download PNG**, then open the file and print it on the printer that holds that label size, choosing the matching paper size and printing at 100% / actual size. **Copy Image** copies it to paste into a label program.

For a plain QR code, use **QR Code** instead; it also offers **Copy Image** and a PNG download. **Copy Link** copies the spot's short link.

![Label](/images/rentals/admin-label.png){width=700px}

![QR Code](/images/rentals/admin-qr.png){width=700px}

To print many labels, tick several spots (or the box at the top of the table) and click **Labels (n)**. Choose the size and click **Download PDF**. The PDF has one label per page in number order, so print it at 100% on the label printer.

![Labels for several spots](/images/rentals/admin-bulk-labels.png){width=700px}

The short link on a label is permanent for that spot. If the preview says the short link is unavailable, click the retry button. If it keeps failing, ask an admin to check the site's public address setting.

## Rental Types

Each type has a **Display Name**, a **Billing Plan (Invoice Option)**, and an **Active** setting. Click **Add Type** (or tick a type and click **Edit**).

Members are billed through the type's billing plan. A type with no plan shows **Not configured**, with a link to **Set up Invoice Option**. Spots of that type cannot be billed correctly until you create the plan under **Billing Options** and choose it on the type. Untick **Active** to stop offering a type for new spots.

![Rental Types](/images/rentals/admin-types.png){width=700px}

## Troubleshooting

| Problem | What to check |
| --- | --- |
| A member cannot request a rental | Their membership must be active, and they must have no past-due invoices. The portal tells them which. |
| A spot does not appear for members | The spot is inactive, already rented (see **Available**), or its type is inactive. |
| A rental shows **Pending Agreement** | The member has not signed the rental agreement yet. They see a banner on the Dues tab. |
| A member is not billed | Check the type's billing plan (**Not configured**) and the invoice in the member's Dues tab. |
| Duplicate or invalid spot number | Numbers must be unique, with no spaces. Use a hyphen. |
| A request is sitting unapproved | Check the Members Relations Channel setting in Portal Settings, and that the channel exists. |
| A label's QR link does not work | Confirm the spot is active, then retry the short link. |

## See also

- [Rent a Storage Space](/digital-makerspace/members/rent-a-space) (the member side)
- [Billing options](/digital-makerspace/admin/billing-options)
- [Storage Rentals](/rentals)
