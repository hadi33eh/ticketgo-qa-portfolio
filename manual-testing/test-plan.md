# TicketGo — Manual Test Plan

**Project:** TicketGo (Fictional Ticket Booking System)  
**Document Version:** 1.0  
**Test Level:** System Testing  
**Test Approach:** Risk-Based Manual Testing  
**Status:** Draft — Not Executed

---

## 1. Objective

The objective of this test plan is to verify the core functionality of TicketGo, including user authentication, registration, ticket booking, pricing, and cancellation.

The testing process aims to identify functional defects, validate business rules, and reduce release risks.

## 2. Scope

### In Scope

- User registration with valid and invalid inputs
- Login with valid and invalid credentials
- Ticket selection and quantity limits
- Passenger information management
- Ticket price calculation
- Discount code validation
- Booking confirmation and tracking code
- Ticket cancellation and booking status changes
- Basic regression testing

### Out of Scope

- Large-scale performance and load testing
- Penetration testing
- Real payment gateway integration testing
- Production infrastructure testing
- Mobile native application testing

## 3. Test Strategy

The following testing approaches are planned:

| Test Type | Purpose |
|---|---|
| Functional Testing | Verify business requirements |
| Positive Testing | Confirm valid user actions |
| Negative Testing | Verify rejection of invalid inputs |
| Exploratory Testing | Discover unexpected behavior |
| Regression Testing | Check existing functionality after changes |
| Smoke Testing | Verify critical functions before detailed testing |

### Test Design Techniques

- Equivalence Partitioning (EP)
- Boundary Value Analysis (BVA)
- Decision Table Testing
- State Transition Testing

Testing will prioritize authentication, booking accuracy, pricing, and cancellation because failures in these areas could have a high impact on users.

## 4. Test Environment

**Environment:** Planned staging/test environment

**Platform:** Web application

**Browsers:** Chrome and Firefox

**Test Data:**
- Valid and invalid test user accounts
- Available ticket inventory
- Sample passenger information
- Valid, invalid, and expired discount codes
- Pending, Confirmed, and Cancelled bookings

Actual environment details must be confirmed before execution.

## 5. Entry Criteria

Testing can begin when:

1. A stable test build is available.
2. The test environment is accessible.
3. Core requirements are documented.
4. Required test accounts and test data exist.
5. Critical dependencies are available or appropriately simulated.

If mandatory entry criteria are not met, affected testing activities will be marked Blocked.

## 6. Exit Criteria

Testing may be considered complete when:

1. All planned critical test cases have been executed.
2. No unresolved release-blocking defects remain.
3. At least 95% of planned test cases have been executed.
4. All remaining known defects have been reviewed and their risks accepted by the responsible team.
5. A test summary report has been prepared.

These criteria are proposed for training purposes and require stakeholder agreement in a real project.

## 7. Defect Management

Defects will be documented with:

- Bug ID and title
- Environment
- Preconditions
- Steps to reproduce
- Expected and actual results
- Severity and priority
- Evidence, when available
- Current defect status

Fictional sample defects will be clearly distinguished from actual observed defects.

## 8. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| QA Engineer | Design and execute tests, report defects |
| Developer | Investigate and fix confirmed defects |
| Product Owner | Clarify requirements and acceptance criteria |
| QA Lead / Release Owner | Review test results and release risks |

These roles represent a proposed team structure, not an actual TicketGo organization.

## 9. Risks and Mitigation

| Risk | Impact | Mitigation |
|---|---|---|
| Test environment unavailable | Testing blocked | Confirm readiness before execution |
| Incomplete requirements | Incorrect test expectations | Clarify acceptance criteria |
| Insufficient test data | Reduced coverage | Prepare representative datasets |
| Late code changes | Regression defects | Perform risk-based regression |
| Limited testing time | Critical defects missed | Prioritize high-risk functionality |

## 10. Test Deliverables

The planned deliverables include:

- Test scenarios
- Login and registration test cases
- EP and BVA test designs
- Decision tables
- State transition tests
- Exploratory testing charters
- Bug reports
- Test execution results
- Test summary report

## 11. Test Schedule

| Phase | Planned Activity |
|---|---|
| Phase 1 | Requirements review and test planning |
| Phase 2 | Test design and test data preparation |
| Phase 3 | Smoke and functional testing |
| Phase 4 | Exploratory and negative testing |
| Phase 5 | Defect retesting and regression |
| Phase 6 | Test summary and closure |

Exact dates and durations will be defined when a real project schedule is available.

## 12. Approval and Execution Status

**Document Status:** Draft  
**Approval Status:** Not Approved  
**Test Execution Status:** Not Started

This document is a training artifact based on fictional TicketGo requirements. It does not represent an approved or executed test plan for a live product.
