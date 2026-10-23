---
title: Slack Identity Conflicts
description: "For admins: resolve cases where two Slack accounts share one member's email by choosing which stays linked."
published: true
date: 2026-10-23T15:00:00.000Z
tags: portal, admin, slack
editor: markdown
dateCreated: 2026-10-23T15:00:00.000Z
---

# Slack Identity Conflicts

The portal links each member to a Slack account by email. When a member has two Slack accounts with the same email, only one can be linked. The sync skips the other instead of failing, and it appears here for an admin to decide.

Open **Portal Settings**, choose the **Slack** tab, and choose **Resolve Slack Conflicts**. Only admins can use this page. If there is nothing to resolve it says "No Slack identity conflicts right now."

Each conflict shows the member's name, which links to their profile, and two Slack accounts:

- **Currently linked:** the account the member has now.
- **Not linked (conflict):** the other account with the same email.

Choose one of:

- **Keep this one** (under the linked account) keeps the current link. The other account is dismissed as a duplicate.
- **Link this one** (under the other account) switches the member to it. The current account is unlinked.

Either way you are asked to confirm, and the choice **cannot be undone from this screen**. The account that loses is not offered again or reconnected automatically. Only a developer with database access could reverse it. No change is made in Slack itself. Make sure you pick the account the member actually uses. If you are not sure, ask the member first.

Each resolution is recorded in the [audit log](/digital-makerspace/admin/audit-log).

## Troubleshooting

| Problem | What to check |
| --- | --- |
| A member is not getting Slack messages | Look for their name here. A conflict stops the sync from linking one of their accounts. |
| The wrong account stayed linked | It cannot be reversed here. Ask a developer to fix it. |

*Last reviewed: October 2026*
