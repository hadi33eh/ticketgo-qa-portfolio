# TicketGo — Registration Test Cases

**Module:** Registration

**Test Type:** Manual Testing

**Execution Status:** Not Run

## Scope

This document covers positive and negative registration test cases.

## Requirements

- Mobile number must contain 11 digits and start with 09.
- Password must contain at least 8 characters.
- Password confirmation must match the original password.
- Accepting terms and conditions is mandatory.
- The mobile number must not already be registered.

## Test Cases

### TC-REG-001 — Successful Registration

**Type:** Positive

**Preconditions:** Registration page is available. The test mobile number is not already registered.

**Test Data:**
- Mobile: Valid unused 11-digit number starting with 09
- Password: `Test12345`
- Confirm Password: `Test12345`
- Accept Terms: Yes

**Steps:**
1. Open the Registration page.
2. Enter the valid mobile number.
3. Enter the password and matching confirmation.
4. Accept the terms and conditions.
5. Click Register.

**Expected Result:** Registration succeeds and the user receives confirmation.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-002 — Mobile Number Shorter Than 11 Digits

**Type:** Negative

**Preconditions:** Registration page is available.

**Test Data:** Mobile: `0912345678`; other fields valid.

**Steps:**
1. Open Registration.
2. Enter the 10-digit mobile number.
3. Fill all other fields correctly.
4. Click Register.

**Expected Result:** Registration is rejected due to invalid mobile number length.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-003 — Already Registered Mobile Number

**Type:** Negative

**Preconditions:** A test account already exists with the chosen mobile number.

**Test Data:** Existing registered mobile number; other fields valid.

**Steps:**
1. Open Registration.
2. Enter the existing mobile number.
3. Fill the remaining fields correctly.
4. Click Register.

**Expected Result:** Duplicate registration is prevented and an appropriate error is displayed.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-004 — Password Shorter Than 8 Characters

**Type:** Negative

**Preconditions:** Registration page is available.

**Test Data:** Password: `Ab1234`; Confirm Password: `Ab1234`; other fields valid.

**Steps:**
1. Open Registration.
2. Enter a valid unused mobile number.
3. Enter the 6-character password in both password fields.
4. Accept the terms and click Register.

**Expected Result:** Registration is rejected due to insufficient password length.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-005 — Password Confirmation Mismatch

**Type:** Negative

**Preconditions:** Registration page is available.

**Test Data:**
- Password: `Test12345`
- Confirm Password: `Test54321`
- Other fields: Valid

**Steps:**
1. Open Registration.
2. Fill in a valid unused mobile number.
3. Enter different password and confirmation values.
4. Accept the terms and click Register.

**Expected Result:** Registration is rejected because the passwords do not match.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-006 — Terms Not Accepted

**Type:** Negative

**Preconditions:** Registration page is available.

**Test Data:** All fields valid; Accept Terms: No.

**Steps:**
1. Open Registration.
2. Fill in all required fields correctly.
3. Leave the terms checkbox unchecked.
4. Click Register.

**Expected Result:** Registration is prevented until the terms are accepted.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-007 — Mobile Number Longer Than 11 Digits

**Type:** Negative

**Preconditions:** Registration page is available.

**Test Data:** Mobile: `091234567890`; other fields valid.

**Steps:**
1. Open Registration.
2. Enter the 12-digit mobile number.
3. Complete the other fields correctly.
4. Click Register.

**Expected Result:** Registration is rejected due to invalid mobile number length.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-008 — Empty Mobile Number

**Type:** Negative

**Preconditions:** Registration page is available.

**Test Data:** Mobile: Empty; other fields valid.

**Steps:**
1. Open Registration.
2. Leave the mobile number field empty.
3. Fill the remaining fields correctly.
4. Click Register.

**Expected Result:** Registration is prevented and the mobile number is identified as required.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-009 — Password Exactly 8 Characters

**Type:** Positive

**Preconditions:** Registration page is available. The mobile number is unused.

**Test Data:**
- Password: `Test1234`
- Confirm Password: `Test1234`
- Other fields: Valid

**Steps:**
1. Open Registration.
2. Enter a valid unused mobile number.
3. Enter the 8-character password in both password fields.
4. Accept the terms and click Register.

**Expected Result:** Registration succeeds because the minimum password length is satisfied.

**Actual Result:** Not Executed  
**Status:** Not Run

---

### TC-REG-010 — Invalid Mobile Number Prefix

**Type:** Negative

**Preconditions:** Registration page is available.

**Test Data:** Mobile: `08123456789`; other fields valid.

**Steps:**
1. Open Registration.
2. Enter the mobile number starting with 08.
3. Complete the other fields correctly.
4. Click Register.

**Expected Result:** Registration is rejected because the number does not start with 09.

**Actual Result:** Not Executed  
**Status:** Not Run
