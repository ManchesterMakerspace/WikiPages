---
title: Paid Membership Months
description: Reviewing and increasing the continuous paid membership count on a member profile.
published: true
date: 2026-11-16T22:00:00.000Z
tags: portal, admin, membership
editor: markdown
dateCreated: 2026-11-16T22:00:00.000Z
---

# Paid Membership Months

The profile shows **Continuous paid membership: N months**. Admins and Board can
read another member's count. Only an Admin can use **Increase paid membership
months**; Board and Resource Manager roles cannot correct it.

Before correcting a count, review the member's receipts, payment application and
refund history. **Estimated history** means older source records or continuity
are incomplete. Prepaid terms count immediately when membership duration is
applied. A first-fob-held payment counts when released. Admin Renew and earned
extensions add no paid months. A 240-hour lapse or revocation resets the count.
The profile refreshes the count after its status or expiration changes.

If a confirmed cash/check receipt is recorded but its membership time was not
applied because accounting failed, retry settling that same invoice after
checking its receipt and fob status. The retry applies the recorded payment;
for a recurring invoice it also creates the next billing cycle once. Do not
collect a second payment. A new payment attempt after a processor settlement
decline is tracked separately from the reversed charge.

1. Open the member's profile and choose **Increase paid membership months**.
2. Review **Current value**. Enter a greater whole number in **Proposed months**.
3. Enter a **Correction reason** explaining the evidence. It is saved in the
   audit log with the actor, member and old/new balance.
4. Choose **Save increase**. The profile shows the updated count and a success
   message. The correction does not change expiration, payment charges or access.

If another payment, refund or correction changes the value while the dialog is
open, the current value refreshes. Review it and the proposed correction before
saving again. Use **Retry** for a failed read. A correction cannot proceed while
the member is revoked, has no expiration date, or is at/past the 240-hour lapse
deadline. Restore the appropriate eligibility/expiration first; doing so does
not recover a previous paid streak automatically.

This control only increases the balance. Contact the maintainer if verified
history needs a different repair. See [Troubleshooting](/digital-makerspace/troubleshooting)
and [Audit Log](/digital-makerspace/admin/audit-log).
