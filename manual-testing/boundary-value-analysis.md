# TicketGo — Boundary Value Analysis

**Module:** Booking  
**Technique:** Boundary Value Analysis (BVA)  
**Status:** Test Design — Not Executed

## Requirements

- A booking must contain between 2 and 6 passengers.
- Tickets can be booked from 1 to 30 days in advance.
- Both minimum and maximum limits are inclusive.

## Boundary Test Scenarios

| ID | Input | Boundary | Expected Result |
|---|---|---|---|
| BVA-001 | 1 passenger | Below minimum | Rejected |
| BVA-002 | 2 passengers | Minimum | Accepted |
| BVA-003 | 3 passengers | Above minimum | Accepted |
| BVA-004 | 7 passengers | Above maximum | Rejected |
| BVA-005 | 0 days ahead | Below minimum date | Rejected |
| BVA-006 | 1 day ahead | Minimum date | Accepted |
| BVA-007 | 30 days ahead | Maximum date | Accepted |
| BVA-008 | 31 days ahead | Above maximum date | Rejected |

## Additional Boundary Values

For broader three-point boundary coverage:

**Passenger count:** 1, 2, 3, 5, 6, 7

**Booking date (days ahead):** 0, 1, 2, 29, 30, 31

## Notes

These are fictional booking requirements defined for QA practice. All scenarios are designed but not yet executed.

An Accepted result indicates that the input satisfies the specific boundary rule, assuming other booking requirements are met.
