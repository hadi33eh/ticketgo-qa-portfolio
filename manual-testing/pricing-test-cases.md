# TicketGo — Pricing & Discount Test Cases

**Project:** TicketGo (Fictional Booking System)  
**Module:** Pricing and Discounts  
**Execution Status:** Not Run

## Assumptions

- Each ticket has a base price of 1,000 units.
- A valid 20% discount code is available.
- Discounts apply to the total ticket price.
- Expired and invalid discount codes must be rejected.
- Final prices cannot be negative.

## Test Cases

| ID | Scenario | Expected Result | Status |
|---|---|---|---|
| TC-PRICE-001 | Select one ticket without a discount | Total price is 1,000 units | Not Run |
| TC-PRICE-002 | Select three tickets without a discount | Total price is 3,000 units | Not Run |
| TC-PRICE-003 | Apply a valid 20% discount to a 1,000-unit booking | Final price is 800 units | Not Run |
| TC-PRICE-004 | Apply a valid 20% discount to a 3,000-unit booking | Final price is 2,400 units | Not Run |
| TC-PRICE-005 | Apply an expired discount code | Discount is rejected and original price remains | Not Run |
| TC-PRICE-006 | Apply an invalid discount code | Discount is rejected and original price remains | Not Run |
| TC-PRICE-007 | Increase ticket quantity from one to two | Total price updates from 1,000 to 2,000 units | Not Run |
| TC-PRICE-008 | Decrease ticket quantity from three to two | Total price updates from 3,000 to 2,000 units | Not Run |
| TC-PRICE-009 | Remove an applied 20% discount from a one-ticket booking | Original price of 1,000 units is restored | Not Run |
| TC-PRICE-010 | Submit a manipulated price value below zero | Negative final price is rejected and the booking is not completed | Not Run |

## Test Execution Notes

- All cases are designed but not executed.
- The amounts and discount rules are fictional test data.
- Actual prices, taxes, service fees, and discount restrictions must be confirmed from real requirements before execution.
- A complete executable test case should also include preconditions, test data, detailed steps, and actual results.
