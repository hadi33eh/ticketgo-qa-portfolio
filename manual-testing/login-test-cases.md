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
