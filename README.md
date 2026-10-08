# Manual Testing Portfolio – E-Commerce Web Application

## Project Overview

This project demonstrates manual software testing activities performed on the Practice Software Testing e-commerce web application.

The purpose of the project is to practice and demonstrate fundamental QA skills such as test planning, test scenario creation, test case design, test execution, defect reporting, and basic test design techniques.

Tested application: Practice Software Testing

---

## Scope

The following areas were included in the test scope:

- Login
- User Registration
- Product Search
- Shopping Cart

The following areas were excluded from the scope:

- Payment Processing
- API Testing
- Database Testing
- Performance Testing
- Security Testing

---

## Testing Activities

The following testing activities were performed during this project:

- Test planning
- Test scenario design
- Test case creation
- Functional testing
- Positive testing
- Negative testing
- Exploratory testing
- Test execution
- Bug reporting
- Equivalence Partitioning
- Boundary Value Analysis

---

## Test Artifacts

The repository contains the following test documentation:

### Test Plan
- Project scope
- Test objectives
- Entry and exit criteria
- Test environment
- Test deliverables

### Test Scenarios
High-level test scenarios were created for:

- Login
- Registration
- Product Search
- Shopping Cart

### Test Cases
Detailed test cases were created and executed for:

- Login
- Registration
- Product Search
- Shopping Cart

### Bug Reports
Defects identified during testing were documented with:

- Steps to reproduce
- Actual result
- Expected result
- Severity
- Priority
- Evidence
- Related test case

### Test Design Techniques

The following techniques were practiced:

- Equivalence Partitioning
- Boundary Value Analysis

---

## Example Defects

### BUG_001 – Incorrect Password Validation Message

A password without a required special symbol was rejected correctly, but the displayed validation message did not accurately describe the missing requirement.

Expected behavior:
The user should be informed that the password must contain at least one special symbol.

Actual behavior:
The application displayed:

`Password must not contain invalid characters`

---

### BUG_002 – Shopping Cart Not Synchronized Across Browser Tabs

A product added to the shopping cart was visible in the original browser tab but was not visible when the same application was opened in another tab.

The authentication state was synchronized between browser tabs, while the shopping cart state was not.

---

## Test Design Examples

### Equivalence Partitioning

Password validation was divided into valid and invalid input groups, including:

- Valid password
- Password shorter than minimum length
- Missing uppercase letter
- Missing lowercase letter
- Missing number
- Missing special symbol

### Boundary Value Analysis

The password minimum length requirement was tested using:

- 7 characters → Rejected
- 8 characters → Accepted
- 9 characters → Accepted

---

## Test Environment

- Operating System: Windows 11
- Browser: Google Chrome
- Testing Type: Manual Testing
- Application: Practice Software Testing

---

## Tools Used

- Git
- GitHub
- Google Chrome
- Markdown

---

## Repository Structure

```text
manual-testing-ecommerce
│
├── README.md
│
├── test-plan
│   └── Test-Plan.md
│
├── test-scenarios
│   └── Test-Scenarios.md
│
├── test-cases
│   ├── Login-Test-Cases.md
│   ├── Register-Test-Cases.md
│   ├── Search-Test-Cases.md
│   └── Cart-Test-Cases.md
│
├── bug-reports
│   ├── Bug-Reports.md
│   └── evidence
│
└── test-design
    ├── Equivalence-Partitioning.md
    └── Boundary-Value-Analysis.md

---

## What I Learned

During this project, I practiced how to:

- Convert high-level scenarios into detailed test cases
- Define preconditions, test data, expected results, and actual results
- Distinguish between positive and negative testing
- Avoid making assumptions when requirements are unclear
- Identify missing or ambiguous requirements
- Execute test cases against a real application
- Document reproducible defects
- Determine severity and priority
- Link failed test cases with related bug reports
- Apply Equivalence Partitioning and Boundary Value Analysis
- Use Git and GitHub to manage QA documentation

---

## Project Status

Completed.

This project represents my first structured manual software testing portfolio project and will be followed by additional projects focusing on API testing, SQL validation, and test automation.
