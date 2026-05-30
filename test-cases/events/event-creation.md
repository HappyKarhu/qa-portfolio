# Test Cases - Organizer event creation

## Feature: Organizer core feature

## 📌 Precondition
User is logged in as Organizer.
From the landing page, click "Create event" to open the registration form.
Unless stated otherwise, all steps assume the Create a new event page is already open.

---

## Simple events

### When creating choose simple event.
---
## 🟠 TC-OE1: Create event creation with valid data and avatar

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

## 🟡 TC-OE2: Create event without image

### Steps:
1. Enter all required fields
2. Do not upload event image
3. Click "Create event"

### Expected Result:
Event is created successfully
Default event image is used.

---

## 🟢 TC-OE3 Create event with missing required fields

### Steps:
1. Leave the title empty
2. Do not choose a date
3. Click "Create event"

### Expected result:
Validation errors for each required field

---

## 🔴 TC-OE4: Capacity unvalid

### Steps:
1. Enter all required fields (with today's date)
2. Set capacity 0 or negative number
3. Click "Create event"

### Expected result:
Error message "The capacity field must be at leats 1"

---

## 🟣 TC-OE5: Start date in the past

### Steps:
1. Enter all required fields
2. Set start Date to yesterday
3. Set the end Date to today
4. Click "Create event"

### Expected result:
Error message: Start date must be today or a future date.

---

## 🟣 TC-OE6: End date before start date

### Steps:
1. Enter all required fields
2. Set start Date to tomorrow
3. Set the end Date to today
4. Click "Create event"

### Expected result:
Error message: "nd date must be after or equal to start date." is displayed and event is not created.

---







