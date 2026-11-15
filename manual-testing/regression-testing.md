# TicketGo — Regression Testing Plan

**Project:** TicketGo (Fictional Booking System)  
**Module:** Booking / Pricing / Discounts  
**Status:** Planned — Not Executed

## Change Under Test

A hypothetical defect in discount calculation has been fixed.

Previously, a valid 20% discount did not reduce the booking price.

## Retesting

| ID | Scenario | Expected Result | Status |
|---|---|---|---|
| RT-001 | Apply valid 20% discount to a booking worth 1000 units | Final price is 800 units | Not Run |

## Regression Test Suite

| ID | Scenario | Expected Result | Status |
|---|---|---|---|
| RG-001 | Calculate price for one ticket without discount | Correct base price displayed | Not Run |
| RG-002 | Calculate total for three tickets | Correct sum displayed | Not Run |
| RG-003 | Apply expired discount code | Discount rejected | Not Run |
| RG-004 | Increase ticket count after applying discount | Final price recalculated correctly | Not Run |
| RG-005 | Remove an applied discount code | Original price restored | Not Run |

## Test Execution Report

**Execution Date:** Not Scheduled  
**Environment:** Not Available  
**Build Version:** Not Available  
**Execution Status:** Not Started

| Metric | Value |
|---|---:|
| Total Planned Tests | 6 |
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Run | 6 |

## Risks

- Incorrect final amount after discounts
- Discounts incorrectly applied to multiple tickets
- Expired discount codes accepted
- Pricing not recalculated after quantity changes

## Notes

This document contains a hypothetical change, planned retesting, and regression scenarios.

No tests have been executed against a live TicketGo application.

The execution report is a pre-execution baseline, not evidence of a completed test run.
