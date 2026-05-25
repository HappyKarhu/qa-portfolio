# Test Cases – User Login

## Feature: User Login

## 📌 Precondition
All test cases start from the landing page.
From the landing page, click "Log in" to open the login form.
Unless stated otherwise, all steps assume the login page is already open.

---
## 🟠 TC-U1: User log in

### Steps:
1. From landing page go to Login
2. Enter valid email: tester_organizer1@test.com
3. Enter password: Password123
4. Click Log in button

### Expected Result:
Redirect goes to user dashboard 

---

## 🟠 TC-U2: User log in with unknown credetals

### Steps:
1. Enter unregistered email: unregistered@user.com
2. Enter password: Password123
3. Click Log in button

### Expected Result:
Error message: "These credentials do not match our records."

---

## 🟠 TC-U3: User log in with invalid email format

### Steps:
1. Enter valid email: tester-test.com
3. Enter password: Password123
4. Click Log in button

### Expected Result:
Error message

---

## 🟠 TC-U4: User log in with wrong password

### Steps:
1. Enter valid email: tester_organizer1@test.com
2. Enter wrong password: 123123123
3. Click Log in button

### Expected Result:
message: "These credentials do not match our records."

---

## 🟠 TC-U5: User log in with empty fields

### Steps:
1. Click Log in button without any writtting into fields

### Expected Result:
Message that this are required fields.
