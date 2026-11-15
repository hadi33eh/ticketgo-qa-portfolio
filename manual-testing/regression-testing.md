# TicketGo — Regression Testing

**Project:** TicketGo (Fictional Ticket Booking System)  
**Module:** Booking / Pricing / Discounts  
**Test Type:** Retesting and Regression Testing  
**Execution Status:** Not Run

## 1. Objective

Verify that a hypothetical discount calculation defect has been fixed and that related pricing functionality continues to work correctly.

## 2. Change Under Test

**Related Bug:** BUG-002

**Description:** Applying a valid 20% discount to a booking worth 1,000 units previously did not update the final price.

**Expected Fix:** A valid 20% discount reduces the total from 1,000 to 800 units.

**Fix Status:** Hypothetically fixed for this training exercise.

## 3. Retesting

| ID | Scenario | Expected Result | Status |
|---|---|---|---|
| RT-001 | Apply valid 20% discount to a booking worth 1,000 units | Final total is 800 units | Not Run |

## 4. Regression Test Suite

| ID | Scenario | Expected Result | Status |
|---|---|---|---|
| RG-001 | Book one ticket without discount | Correct base price displayed | Not Run |
| RG-002 | Book three tickets without discount | Correct total price calculated | Not Run |
| RG-003 | Apply an expired discount code | Discount is rejected | Not Run |
| RG-004 | Change ticket quantity after applying a valid discount | Total price is recalculated correctly | Not Run |
| RG-005 | Remove an applied discount code | Original price is restored | Not Run |

## 5. Test Execution Report

**Environment:** Not Available  
**Build Version:** Not Available  
**Execution Date:** Not Scheduled

| Metric | Count |
|---|---:|
| Total Tests | 6 |
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Run | 6 |
| Execution Rate | 0% |

## 6. Risks

- Incorrect discount calculations
- Incorrect total after changing ticket quantity
- Expired discount codes being accepted
- Original price not restored after removing discount

## 7. Conclusion

All test scenarios have been designed but not executed.

The defect fix has not been verified against a real application.

This document is a training artifact based on fictional TicketGo requirements.
