# TicketGo — Manual Test Scenarios

**Project:** TicketGo (Fictional Booking System)  
**Modules:** Login, Booking, Cancellation  
**Status:** Draft — Requirements Pending Validation

## Login Scenarios

| ID | Test Scenario | Type |
|---|---|---|
| TS-001 | Verify that login is rejected when authentication credentials are invalid. | Negative |
| TS-002 | Verify that valid discount codes update the total booking price correctly. | Positive |
| TS-003 | Verify that a tracking code is displayed after a successful booking. | Positive |
| TS-004 | Verify that passenger information is saved for future bookings when the user explicitly chooses to save it. | Positive |
| TS-005 | Verify that ticket prices are calculated according to the applicable pricing rules. | Functional |
| TS-006 | Verify that users cannot book more than five tickets in a single booking. | Negative |
| TS-007 | Verify that separate passenger details are collected for each selected ticket. | Positive |
| TS-008 | Verify that duplicate ticket issuance is prevented when prohibited by business rules. | Negative |
| TS-009 | Verify that authentication is required before accessing a user account. | Negative |
| TS-010 | Verify that entered booking information is preserved after a page refresh when required by the specification. | Functional |
| TS-011 | Verify that the total price updates when tickets are added or removed. | Functional |
| TS-012 | Verify that users can select an individual passenger when submitting a cancellation request. | Positive |

## Notes

- These scenarios were designed for a fictional ticket-booking system.
- Specific pricing, duplicate-ticket, and refresh-persistence rules require confirmation.
- Execution results will be documented separately.
- No scenarios in this file are marked as executed.
