# Test Plan — Project 01 (Web E-commerce Application)

## 1. Document Information

- Project Name: Project 01 — Web Application Testing (E-commerce)
- Document Type: Test Plan
- Version: 1.0
- Author: Ana Roberta Mota
- Date: [Insert date]

---

## 2. Objective

The objective of this test plan is to define the testing strategy, scope, approach, resources, and schedule for validating the main functional workflows of a web-based e-commerce application.

The goal is to ensure that the system behaves according to requirements, supports expected user flows, and handles common input validation scenarios.

---

## 3. Scope

### 3.1 In Scope

The following functionalities are included in the scope of testing:

- User Registration
- User Login / Logout
- Product browsing (categories, listing)
- Product search and filtering
- Product details page
- Add to cart / remove from cart
- Update product quantity in cart
- Checkout flow (basic validation)
- Order confirmation page

---

### 3.2 Out of Scope

The following areas are excluded from this test cycle:

- Payment gateway integration testing (external service)
- Performance testing (load/stress)
- Security testing (penetration testing)
- Automation testing (Selenium/Cypress)
- Database testing
- Compatibility testing on multiple devices/browsers (only basic coverage)

---

## 4. Test Approach

Testing will be performed manually based on functional requirements and expected user workflows.

The test approach includes:

- Requirement-based testing
- Workflow-based testing (UAT)
- Positive and negative test scenarios
- Boundary value checks for input fields (basic)
- Defect reporting with evidence and reproducible steps

---

## 5. Test Types

The following test types will be performed:

### 5.1 Functional Testing
Validation of expected behaviors based on requirements and user flows.

### 5.2 Smoke Testing
Quick validation to ensure that critical functionalities work after builds or updates.

### 5.3 Regression Testing (Basic)
Execution of critical test cases to ensure that fixes or changes did not break existing features.

### 5.4 Exploratory Testing
Unscripted testing to identify unexpected behavior, UI issues, or edge-case defects.

### 5.5 UAT Validation
Validation of end-to-end workflows from the user perspective.

---

## 6. Test Environment

- Application Type: Web Application
- Browsers: Google Chrome, Mozilla Firefox
- Operating System: Windows / macOS
- Testing Method: Manual testing
- Test Data: Dummy users, sample products

---

## 7. Test Deliverables

The following QA artifacts will be produced:

- Test Plan
- Test Cases
- Bug Reports
- Traceability Matrix (RTM)
- Test Summary Report
- Evidence (Screenshots)

---

## 8. Entry Criteria

Testing can start when:

- Test environment is available and stable
- Core requirements are documented
- Test data is available
- Test cases are prepared

---

## 9. Exit Criteria

Testing will be considered complete when:

- All planned test cases have been executed
- All Critical/High severity defects are documented and communicated
- Test Summary Report is completed
- RTM is updated and finalized

---

## 10. Defect Management Process

Defects will be documented using a structured bug report format including:

- Defect ID
- Title / Summary
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity and Priority
- Environment (browser, OS)
- Evidence (screenshots/logs)
- Status (New, Open, In Progress, Fixed, Retest, Closed)

Severity levels:

- Critical: System crash, blocking workflow, data loss
- High: Major functionality not working
- Medium: Partial failure or inconsistent behavior
- Low: Minor UI issues, cosmetic defects

---

## 11. Test Risks

Potential risks during testing:

- Lack of detailed requirements may impact test coverage
- Environment instability may delay execution
- Limited browser/device coverage may hide compatibility defects
- Test data limitations may reduce scenario depth

---

## 12. Assumptions

- Application is accessible for testing
- Basic requirements are available (even if simplified)
- Test environment has stable internet access

---

## 13. Test Roles and Responsibilities

- QA Tester: Ana Roberta Mota  
  Responsibilities: test planning, test case design, execution, defect reporting, documentation, reporting.

---

## 14. Schedule (High-Level)

- Test Planning: 1 day
- Test Case Design: 2 days
- Test Execution: 3–5 days
- Bug Reporting and Retesting: ongoing during execution
- Final Reporting: 1 day

---

## 15. Approval

This test plan is created for QA portfolio demonstration purposes and does not represent confidential or proprietary software.
