# TicketGo — Login Test Cases

**Module:** Login  
**Test Type:** Manual Testing  
**Execution Status:** Not Run

## TC-LOGIN-001 — Successful Login

**Type:** Positive

**Preconditions:**
- Login page is available.
- An active test user account exists.

**Test Data:**
- Mobile: Valid registered test mobile number
- Password: Valid password for the test account

**Steps:**
1. Open the Login page.
2. Enter the registered mobile number.
3. Enter the correct password.
4. Click Login.

**Expected Result:**
The user successfully logs in and is redirected to their account.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-002 — Login with Incorrect Password

**Type:** Negative

**Preconditions:**
- Login page is available.
- An active test user account exists.

**Test Data:**
- Mobile: Valid registered test mobile number
- Password: Incorrect password

**Steps:**
1. Open the Login page.
2. Enter the registered mobile number.
3. Enter an incorrect password.
4. Click Login.

**Expected Result:**
Login is rejected and an appropriate authentication error is displayed.

**Actual Result:** Not Executed  
**Status:** Not Run


---

## TC-LOGIN-003 — Login with Unregistered Mobile Number

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: Valid-format but unregistered test number
- Password: `Test12345`

**Steps:**
1. Open the Login page.
2. Enter the unregistered mobile number.
3. Enter the password.
4. Click Login.

**Expected Result:** Login is rejected and an appropriate error is displayed.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-004 — Login with Mobile Number Shorter Than 11 Digits

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: `0912345678`
- Password: `Test12345`

**Steps:**
1. Open the Login page.
2. Enter the 10-digit mobile number.
3. Enter the password.
4. Click Login.

**Expected Result:** Login is rejected and a mobile-number validation error is displayed.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-005 — Login with Mobile Number Longer Than 11 Digits

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: `091234567890`
- Password: `Test12345`

**Steps:**
1. Open the Login page.
2. Enter the 12-digit mobile number.
3. Enter the password.
4. Click Login.

**Expected Result:** The system prevents login using an invalid-length mobile number.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-006 — Login with Invalid Mobile Prefix

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: `08123456789`
- Password: `Test12345`

**Steps:**
1. Open the Login page.
2. Enter the mobile number.
3. Enter the password.
4. Click Login.

**Expected Result:** Login is rejected because the mobile number does not start with `09`.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-007 — Login with Password Shorter Than 8 Characters

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: Valid registered test number
- Password: `Ab1234`

**Steps:**
1. Open the Login page.
2. Enter the registered mobile number.
3. Enter the 6-character password.
4. Click Login.

**Expected Result:** Login is rejected and an appropriate password validation error is displayed, according to the agreed requirements.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-008 — Login with Empty Mobile Number

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: Empty
- Password: `Test12345`

**Steps:**
1. Open the Login page.
2. Leave the mobile number field empty.
3. Enter the password.
4. Click Login.

**Expected Result:** Login is rejected and the mobile number field is marked as required.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-009 — Login with Empty Password

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: Valid registered test number
- Password: Empty

**Steps:**
1. Open the Login page.
2. Enter the registered mobile number.
3. Leave the password field empty.
4. Click Login.

**Expected Result:** Login is rejected and the password field is marked as required.

**Actual Result:** Not Executed  
**Status:** Not Run

---

## TC-LOGIN-010 — Login with Both Fields Empty

**Type:** Negative  
**Preconditions:** Login page is available.

**Test Data:**
- Mobile: Empty
- Password: Empty

**Steps:**
1. Open the Login page.
2. Leave both fields empty.
3. Click Login.

**Expected Result:** Login is rejected and required-field validation errors are displayed.

**Actual Result:** Not Executed  
**Status:** Not Run
