# TicketGo — Cancellation Test Cases

**Project:** TicketGo (Fictional Ticket Booking System)  
**Module:** Cancellation and Booking Status  
**Execution Status:** Not Run

## Assumptions

- Pending bookings can be cancelled by their owners.
- Confirmed bookings can be cancelled only when more than 24 hours remain before departure.
- Cancellation at exactly 24 hours before departure is not allowed.
- Cancelled bookings cannot be reactivated.
- Only the booking owner can cancel a booking.
- A rejected cancellation must not change the booking status.
- For multi-passenger bookings, individual passenger cancellation is supported.

## Test Cases

| ID | Scenario | Expected Result | Status |
|---|---|---|---|
| TC-CANCEL-001 | Cancel a Pending booking as its owner | Booking status changes to Cancelled | Not Run |
| TC-CANCEL-002 | Cancel a Confirmed booking 48 hours before departure | Cancellation succeeds and status becomes Cancelled | Not Run |
| TC-CANCEL-003 | Attempt cancellation of a Confirmed booking 12 hours before departure | Cancellation is rejected and status remains Confirmed | Not Run |
| TC-CANCEL-004 | Attempt cancellation exactly 24 hours before departure | Cancellation is rejected and status remains Confirmed | Not Run |
| TC-CANCEL-005 | Attempt to cancel an already Cancelled booking | Request is rejected and status remains Cancelled | Not Run |
| TC-CANCEL-006 | Attempt to reactivate a Cancelled booking | Reactivation is rejected and status remains Cancelled | Not Run |
| TC-CANCEL-007 | Attempt to cancel another user's booking | Access is denied and booking status remains unchanged | Not Run |
| TC-CANCEL-008 | Cancel one passenger from a confirmed two-passenger booking more than 24 hours before departure | Selected passenger is cancelled; other passenger remains confirmed | Not Run |
| TC-CANCEL-009 | Refresh the booking details page after successful cancellation | Cancelled status remains correctly displayed | Not Run |
| TC-CANCEL-010 | Submit the same cancellation request twice | The second request does not cause duplicate cancellation effects | Not Run |

## Coverage Notes

These cases cover:
- Valid and invalid cancellation requests
- Cancellation deadline boundaries
- Authorization
- State transitions
- Individual passenger cancellation
- State persistence
- Duplicate requests

## Execution Notes

- All cases are designed but not executed.
- Actual results and evidence must be recorded during real execution.
- All business rules are hypothetical and require confirmation in a real project.
- Detailed test steps, test data, and preconditions should be added before execution.
