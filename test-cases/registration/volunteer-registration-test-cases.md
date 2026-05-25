# Test Cases – Volunteer Registration (Laravel Volunteer Event Platform)

## Feature: Volunteer Registration & Authentication

## 📌 Precondition
All test cases start from the landing page.
From the landing page, click "Register" to open the registration form.
Unless stated otherwise, all steps assume the registration page is already open.

---
## 🟠 TC-1: Successful registration with valid data and avatar

### Steps:
1. Enter valid full name: Tester Volunteer 1
2. Enter valid email: tester_volunteer1@test.com
3. Enter strong password: Password123
4. Choose Register as Volunteer field
5. Upload valid avatar (jpeg,png,jpg,gif,webp)
6. Click Register button

### Expected Result:
User account is created successfully.
User is redirected to dashboard.
Avatar is stored correctly and displayed in profile.

---

## 🟢 TC-2: Registration without avatar (default behavior)

### Steps:
1. Enter valid full name: Tester Volunteer 2
2. Enter valid email: tester_volunteer2@test.com
3. Enter strong password: Password123
4. Choose Register as Volunteer field
5. Click Register button

### Expected Result:
User is created successfully.
System assigns a default avatar automatically.

---

## 🟡 TC-3: Invalid avatar format upload

### Steps:
1. Enter valid full name: Invalid Tester
2. Enter valid email: invalid_tester@test.com
3. Enter strong password: Password123
4. Choose Register as Volunteer field
5. Upload invalid file format (e.g. .txt, .pdf)
6. Click Register button

### Expected Result:
System blocks upload.
Error message displayed:
"Invalid file type. Please upload JPG or PNG image."

---

## 🔴 TC-4: Duplicate email registration

### Steps:
1. Enter email already used in system: VolunteerTester1@test.com
2. Click Register button
   
### Expected Result:
System shows error:
"The email has already been taken."

---

## 🟡 TC-5: Password validation (weak password)

### Steps:
1. Enter full name: Tester
2. Enter email: test@test.com
3. Enter weak password: (123)
4. Click Register button

### Expected Result:
System rejects password and shows validation message: 
"The password field must be at least 8 characters.".

---

## 🟢 TC-6: Empty field validation

### Steps:
1. Submit form without filling any fields

### Expected Result:
Validation errors shown for all required fields.

---

## 🔴 TC-7: Invalid email format validation

### Steps:
1. Enter email: test@
2. Fill other fields correctly
3. Click Register button

### Expected Result:
System shows error: “Invalid email format”

---

## 🔴 TC-8: Password confirmation mismatch

### Steps:
1. Enter password: Password123
2. Enter confirm password: Password124
3. Click Register button

### Expected Result:
System shows error: “Passwords do not match”
