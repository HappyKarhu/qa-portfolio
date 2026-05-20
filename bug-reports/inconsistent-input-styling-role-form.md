# Bug: Inconsistent Input Field Background Colors in Role Creation Form

## Environment
- Application: Volunteer Event Platform
- Module: Event Creation (Sectioned Event)
- Framework: Laravel 13
- Browser: Chrome
- OS: Windows 11

---

## Description
In the Sectioned Event creation form, input fields for **Role Name, Capacity, and Description** use different background colors (green/blue) compared to the rest of the form.

Other input fields follow a consistent standard UI styling, resulting in visual inconsistency within the same form.

---

## Steps to Reproduce
1. Open event creation page
2. Select “Sectioned Event” type
3. Scroll to role input section
4. Observe styling of input fields
5. Compare with other form fields

---

## Actual Result
- Role Name, Capacity, and Description fields use green/blue background styling
- Other input fields use standard consistent styling

---

## Expected Result
All input fields in the form should use consistent background color and styling unless there is a clear functional reason for differentiation.

---

## Severity
Low / Medium

---

## Impact
- Reduces UI consistency and visual polish
- May confuse users about field importance or behavior
- Decreases overall UX quality

---

## Recommendation
Standardize input field styling across the form or clearly define visual rules for different field types.

---

## Attachment
Screenshot: Näyttökuva 2026-05-20 095902.png
