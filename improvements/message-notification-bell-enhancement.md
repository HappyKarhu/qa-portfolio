# Improvement: Show Unread Messages in Notification Bell

## Tracking Information
- Jira Ticket: KAN-7
- Status: In Progress
- Priority: Medium

---

## Environment
- Application: Volunteer Event Platform
- Module: Messaging / Notifications
- Framework: Laravel 13

---

## Description
Currently, unread messages are not included in the notification bell.

Users must manually open a specific event and navigate to the Messages section to check for new messages. This reduces visibility and slows down communication.

---

## Current Behavior
- Notification bell shows system notifications
- New messages are not included
- Users must open each event manually to check messages

---

## Proposed Improvement
- Include unread messages in the notification bell
- Show:
  - Sender name
  - Event name
  - Short message preview
- Display unread message count badge
- Mark messages as read when opened

---

## Expected Benefit
- Improved user experience
- Faster access to communication
- Reduced chance of missing important messages
- More consistent notification system

---

## Priority
Medium

---

## Type
Improvement / Enhancement

---

## Notes
This improvement would align messaging behavior with standard notification UX patterns used in modern web applications.
