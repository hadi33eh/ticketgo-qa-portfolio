# TicketGo — Decision Table Testing

**Module:** Discount Code  
**Technique:** Decision Table Testing  
**Execution Status:** Not Run

## Requirements

A discount code can be applied only when:
- The user is logged in.
- The discount code is valid.
- The discount code has not expired.

All three conditions must be satisfied.

## Conditions

- C1: User is logged in
- C2: Discount code is valid
- C3: Discount code is not expired

## Decision Table

| Rule | C1 | C2 | C3 | Expected Action |
|---|---|---|---|---|
| R1 | Yes | Yes | Yes | Apply Discount |
| R2 | Yes | Yes | No | Reject Discount |
| R3 | Yes | No | Yes | Reject Discount |
| R4 | Yes | No | No | Reject Discount |
| R5 | No | Yes | Yes | Reject Discount |
| R6 | No | Yes | No | Reject Discount |
| R7 | No | No | Yes | Reject Discount |
| R8 | No | No | No | Reject Discount |

## Sample Test Case

**Test Case ID:** TC-DT-001

**Title:** Reject an expired discount code

**Preconditions:**
- User is logged in.
- A valid but expired test discount code exists.

**Steps:**
1. Open the Booking page.
2. Enter the expired discount code.
3. Click Apply.

**Expected Result:** Discount is rejected because the code has expired.

**Actual Result:** Not Executed  
**Status:** Not Run

## Notes

All rules and test cases are based on fictional TicketGo requirements. No live system testing has been performed.
