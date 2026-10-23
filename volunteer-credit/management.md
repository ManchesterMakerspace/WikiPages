---
title: Managing Volunteer Tasks
description: For admins, board members and Resource Managers: create bounty tasks and events, review and award volunteer points, and fix mistakes.
published: true
date: 2026-10-22T16:00:00.000Z
tags: volunteer, admin, bounties, events
editor: markdown
dateCreated: 2020-02-03T21:59:33.128Z
---

# Managing Volunteer Tasks

Volunteer tasks, events and points are managed in the member portal. The old spreadsheet is no longer used. Do not add anything to it. For what members do, see [Volunteering at the Makerspace](/volunteer-credit).

Open **Volunteer** from the portal menu. Admins, board members and Resource Managers see it. It has three tabs: **Credits**, **Bounty Tasks** and **Events**.

Some labels and buttons in this part of the portal use the older word "credit". Read it as volunteer points.

## Bounty Tasks

A bounty task is a job members can claim. Open tasks appear on members' Home pages and on the TVs in the space.

The **Bounty Tasks** tab lists each task with its number, title, description, points value, status and claims. **Filter by Status** narrows the list.

### Create a task

1. Choose **Create Task**.
2. Fill in the **Title** and **Description**, both required.
3. Set the **Credit Value**, which is the points the task is worth. Task creation allows 0.5 to 2 in steps of 0.5.
4. Choose the **Task Type**:
   - **Standard (one-time)**: one member does it once.
   - **Reusable (any member once)**: each member can do it once.
   - **Repeatable (any member, unlimited)**: members can do it as often as they like.
   - **Recurring (repeatable with cooldown)**: it can be done again after a number of days. You enter the **Recurrence Interval (days)**.
5. Optionally choose a **Shop**, and **Prerequisite tool checkouts** that a member needs before they can claim it.
6. Choose **Submit**.

### Task statuses

| Status | What it means |
| --- | --- |
| **Available**, **Reusable**, **Repeatable**, **Recurring** | Open for members to claim. |
| **Claimed** | A member has taken it. |
| **Pending Verification** | The member says it is done and it needs review. |
| **Completed** | It was finished and approved. |
| **Cancelled** | It was withdrawn. |
| **Denied** | The completion was not accepted. |

### Change a task

Tick a task to see what you can do:

- **Edit** changes the title, description, recurrence interval and points value. Admin and board edits to the value have no upper limit, and every edit is recorded in the audit log.
- **Cancel** withdraws a task that is still open.
- **Delete** removes a completed task.

When a member marks a task complete it shows **Pending Verification**. Tick it, check the work, and choose **Verify** to accept it or **Reject** to turn it down. Rejecting asks for a reason. For reusable, repeatable and recurring tasks, choose **View** on the task to see each member's claim, then verify or reject each one. Points are added after review. Members see them in the month after the activity.

## Events

Use events for monthly volunteer and cleanup days and other group work.

1. Open the **Events** tab and choose **Create Event**.
2. Fill in the **Title**, **Description**, **Credit Value** (the points each attendee earns) and **Event Date**. You can also choose a **Shop** and **Prerequisite tool checkouts**.
3. Choose **Submit**.

The list shows each event with its points, attendee count and status. **Filter by Status** switches between **Open** and **Closed**. Tick an event to use:

- **Edit** to change it.
- **Add Attendee** to add a member who came but did not sign up.
- **Manage Attendees** to see who is signed up, and to remove someone.
- **Close Event** when the event is over. Points are issued to the attendees when you close it.

Members join an event from their Home page with **Join Event**.

## The Credits tab

This tab is the log of every award. **Filter by Status** shows all, pending, approved, rejected or reversed entries. Each entry shows the member, what it was for, the points and the status: **Approved**, **Pending**, **Rejected** or **Reversed**.

- **Award Credit** gives a member points directly. Search for the member, enter a positive **Credit Value**, add a **Description**, and choose **Award**. Use it for work that was not a bounty or event.
- **Approve** or **Reject** an entry that is **Pending**.
- **Reverse Credit** undoes an approved entry. It asks for a reason, adds a matching **Reversed** entry, and keeps the history. Use it when something was awarded by mistake.
- **Delete** removes entries. Only people with that permission see it.

Some entries are added automatically. For example, an approver's work on a tool checkout is recorded for them, and reversed if the checkout is later revoked.

## Troubleshooting

| Problem | What to check |
| --- | --- |
| A member cannot claim a task | They may not meet the prerequisite checkouts, or they reported the task themselves. |
| A task is not on the Home page | It may be claimed, cancelled or outside the member's shop. |
| Points are missing | The task may still be **Pending Verification**, or the event may not be closed yet. |
| Points were awarded by mistake | Use **Reverse Credit** and give a reason. |

*Last reviewed: October 2026*
