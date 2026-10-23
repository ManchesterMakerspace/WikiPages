---
title: Partner Discounts
description: How to create a discount for a partner organization's members, give them a sign-up link that applies it, and bill the partner.
published: true
date: 2026-10-22T14:00:00.000Z
tags: partnerships, billing, admin, board
editor: markdown
dateCreated: 2026-10-22T14:00:00.000Z
---

# Partner Discounts

A partner discount lets the members of a partner organization, such as a company's employees, join at a reduced rate. The partner is then billed for the discounted part of their members' memberships. This page is for admins and board members. It shows how to create the discount, make the sign-up link that applies it, and produce the bill.

## 1. Create the discount in Braintree

1. Log in to [Braintree](https://www.braintreegateway.com/login).
2. Choose **Subscriptions** in the header, then **Add Ons / Discounts** in the sub-header.
3. Scroll to the bottom and choose **New Discount**.
4. Enter an **ID** that is unique to the partner. The pattern is the partner name, the subscription period and the percent discount. For example, `PARTNER-QTR-50` is a 50% discount for a partner's members on the quarterly membership.
5. Enter a **Name** that describes who the discount is for. Customers see this name.
6. Calculate and enter the discount **amount** for that membership term.
7. Each membership level and term needs its own discount, so repeat for each one the partner should get.

## 2. Make the sign-up link

The link opens the sign-up form with the right membership and the discount already chosen.

1. Open the makerspace's front page at members.manchestermakerspace.org, without signing in.
2. Choose **Sign Up** beside the membership option the partner's members should get. The sign-up form opens, and the address bar now ends in `/signup?optionId=` followed by a code.
3. Copy the whole address.
4. Add `&discountId=` and the discount ID from step 1 to the end. The result looks like this: `https://members.manchestermakerspace.org/signup?optionId=<option code>&discountId=<discount ID>`.
5. Test it in a private browser window. On the **Membership** step you should see the right membership selected and the discount applied to the total. Do not complete the sign-up.

Make one link for each membership term the partner offers. The option code and the discount ID must match: each discount belongs to one membership term.

## 3. Give the link to the partner

Send each link only to the partner's contact. Anyone who has a link can use the discount, so ask the partner to share it only with the people who qualify. If a link gets out, create a new discount with a new ID, make new links, and stop using the old discount.

## What a partner's member does

1. Open the link and fill in the sign-up form. See [Sign Up](/digital-makerspace/sign-up).
2. On the **Membership** step, check that the correct membership and discount are shown. Do not change the selections. Changing them can cause a mismatch between the membership and the discount.
3. Finish payment as usual.

## 4. Bill the partner

The partner pays for the discounted part of their members' memberships.

1. Sign in as an admin or board member and open **Billing** from the portal menu.
2. Open the **Transactions** tab and choose **Filters**.
3. Choose the date range for the bill, and choose the partner's discounts under **Discount**.
4. Choose **Download Table**.

The file lists each transaction with its discount and the discount amount. The partner owes the total of the discounts. See [Transactions](/digital-makerspace/admin/transactions) for more on the filters.

## See also

- [Billing Options](/digital-makerspace/admin/billing-options)
- [Sign Up](/digital-makerspace/sign-up)

*Last reviewed: October 2026*
