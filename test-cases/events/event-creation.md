# Test Cases - Organizer event creation

## Feature: Organizer core feature

## 📌 Precondition
User is logged in as Organizer.
From the landing page, click "Create event" to open the registration form.
Unless stated otherwise, all steps assume the Create a new event page is already open.

---

## Simple events

---
### 🟠 TC-OE1: Create event creation with valid data and avatar

### Steps:
1. Enter valid Event Name
2. Enter valid Event Description
3. Enter Responsibilities
4. Enter Requirements
5. Enter What to Bring/Wear
6. Select valid Start Date (today)
7. Select valid End Date (today)
8. Enter valid Location
9. Select "Free Event"
10. Select “Simple Event”
11. Enter valid Capacity - -number 2
12. Add tags
13. Set status to "Published"
14. Upload valid event image (jpg/png/jpeg/gif/bmp/webp)
15. Click "Create event"

### Expected Result:
Event is created successfully
Organizer is redirected to event page
Event appears in event listing/organizer dashboard
Uploaded image is uploaded and displayed correctly
Event status is set to Published

---


