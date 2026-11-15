# TicketGo — Sample Bug Reports

**Project:** TicketGo (Fictional Booking System)

**Report Type:** Simulated Defects

**Execution Status:** Not Executed

## BUG-001 — Booking Allows More Than Five Tickets

**Module:** Booking

**Severity:** High

**Priority:** High (assuming this rule is release-critical)

**Environment:** Simulated TicketGo Test Environment

**Preconditions:**
- The user is logged in.
- At least six tickets are available.

**Steps to Reproduce:**
1. Open the Booking page.
2. Select six tickets.
3. Click Confirm Booking.

**Expected Result:**
The system must prevent users from booking more than five tickets in a single reservation.

**Actual Result (Simulated):**

---

## BUG-002 — Discount Code Does Not Update Booking Price

**Module:** Booking / Discounts  
**Severity:** Medium  
**Priority:** High (assuming a promotion is active)  
**Environment:** Simulated TicketGo Test Environment

**Preconditions:**
- The user is logged in.
- The booking total is 1,000 units.
- The `OFF20` discount code is valid and provides a 20% discount.

**Steps to Reproduce:**
1. Open the Booking page.
2. Select tickets with a total price of 1,000.
3. Enter the discount code `OFF20`.
4. Click Apply.

**Expected Result:** The total price updates to 800.

**Actual Result (Simulated):** The total remains 1,000.

**Status:** Sample — Not Reproduced

---

## BUG-003 — Cancelled Passenger Status Reverts After Refresh

**Module:** Booking / Cancellation  
**Severity:** High  
**Priority:** High  
**Environment:** Simulated TicketGo Test Environment

**Preconditions:**
- The user is logged in.
- A confirmed booking exists with two passengers.

**Steps to Reproduce:**
1. Open the booking details.
2. Select one passenger for cancellation.
3. Confirm the cancellation.
4. Observe the success message.
5. Refresh the page.

**Expected Result:** The cancelled passenger's status remains `Cancelled`.

**Actual Result (Simulated):** The status returns to `Confirmed`.

**Status:** Sample — Not Reproduced

---

## BUG-004 — Login Succeeds with an Incorrect Password

**Module:** Authentication  
**Severity:** Critical  
**Priority:** High  
**Environment:** Simulated TicketGo Test Environment

**Preconditions:**
- An active test account exists.
- The Login page is available.

**Steps to Reproduce:**
1. Open the Login page.
2. Enter a registered test mobile number.
3. Enter an incorrect password.
4. Click Login.

**Expected Result:** Login is rejected and an authentication error is displayed.

**Actual Result (Simulated):** The user is successfully authenticated.

**Status:** Sample — Not Reproduced

---

## BUG-005 — Tracking Code Missing After Successful Booking

**Module:** Booking Confirmation  
**Severity:** Medium  
**Priority:** Medium  
**Environment:** Simulated TicketGo Test Environment

**Preconditions:**
- The user is logged in.
- Tickets are available.

**Steps to Reproduce:**
1. Open the Booking page.
2. Select an available ticket.
3. Complete the booking process.
4. Open the confirmation page.

**Expected Result:** A unique booking tracking code is displayed.

**Actual Result (Simulated):** The confirmation page appears without a tracking code.

**Status:** Sample — Not Reproduced

---

## Important Note

All defects in this document are fictional examples created for QA training. No actual defects have been reproduced or verified against a live TicketGo application.
The system successfully accepts a reservation for six tickets.

**Status:** Sample — Not Reproduced

**Notes:**
This is a fictional defect created for QA practice. It has not been verified in a real application.
