# TicketGo — State Transition Testing

**Project:** TicketGo (Fictional Ticket Booking System)  
**Module:** Booking Management  
**Technique:** State Transition Testing  
**Execution Status:** Not Run

## 1. Objective

Verify that booking status changes follow the defined business rules and that invalid transitions are prevented.

## 2. Booking States

| State | Description |
|---|---|
| Pending | Booking created, awaiting successful payment |
| Confirmed | Payment completed and booking confirmed |
| Cancelled | Booking cancelled and no longer active |

## 3. Business Rules

- A successful payment changes a Pending booking to Confirmed.
- A Pending booking can be cancelled.
- A Confirmed booking can be cancelled if cancellation requirements are satisfied.
- A Cancelled booking cannot return to Pending or Confirmed.
- A rejected transition must not change the booking status.

## 4. State Transition Table

| ID | Current State | Event | Expected Next State | Result |
|---|---|---|---|---|
| ST-001 | Pending | Successful payment | Confirmed | Allowed |
| ST-002 | Pending | Cancel booking | Cancelled | Allowed |
| ST-003 | Confirmed | Valid cancellation | Cancelled | Allowed |
| ST-004 | Confirmed | Invalid cancellation request | Confirmed | Rejected |
| ST-005 | Cancelled | Attempt payment | Cancelled | Rejected |
| ST-006 | Cancelled | Attempt reactivation | Cancelled | Rejected |
| ST-007 | Pending | Payment failure | Pending | No transition |
| ST-008 | Confirmed | Attempt duplicate payment | Confirmed | Rejected |

## 5. Sample Test Cases

### TC-ST-001 — Successful Payment

**Preconditions:** A booking exists with Pending status.

**Steps:**
1. Open the booking details.
2. Complete a successful test payment.
3. Check the booking status.

**Expected Result:** Booking status changes from Pending to Confirmed.

**Actual Result:** Not Executed  
**Status:** Not Run

### TC-ST-002 — Cancel Confirmed Booking

**Preconditions:** A Confirmed booking exists and cancellation is allowed.

**Steps:**
1. Open the booking details.
2. Select Cancel.
3. Confirm the cancellation.
4. Check the booking status.

**Expected Result:** Booking status changes from Confirmed to Cancelled.

**Actual Result:** Not Executed  
**Status:** Not Run

### TC-ST-003 — Prevent Reactivation of Cancelled Booking

**Preconditions:** A booking exists with Cancelled status.

**Steps:**
1. Open the cancelled booking.
2. Attempt to reactivate the same booking through an available test interface.
3. Check the booking status.

**Expected Result:** Reactivation is rejected and the booking remains Cancelled.

**Actual Result:** Not Executed  
**Status:** Not Run

## 6. Notes

- TicketGo and its requirements are fictional examples for QA training.
- The transition table represents expected behavior, not observed application results.
- All test cases are designed but have not been executed.
- Additional requirements are needed to define cancellation deadlines, timeout behavior, and payment retries.
