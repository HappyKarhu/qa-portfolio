# Test Cases – User Registration

## Feature: User Registration

---

## Test Case 1: Successful Registration

**Steps:**
1. Open registration page
2. Enter valid name
3. Enter valid email
4. Enter valid password
5. Submit form

**Expected Result:**
User account is created successfully and redirected to dashboard.

---

## Test Case 2: Duplicate Email Validation

**Steps:**
1. Open registration page
2. Enter existing email
3. Submit form

**Expected Result:**
System shows error: "The email has already been taken."

---

## Test Case 3: Empty Fields Validation

**Steps:**
1. Submit form with empty fields

**Expected Result:**
Validation errors are shown for required fields.

---

## Test Case 4: Password Strength Validation

**Steps:**
1. Enter weak password
2. Submit form

**Expected Result:**
System rejects weak password and shows validation message.
