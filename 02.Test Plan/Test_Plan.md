# Test Plan
## 1. Document Information

| Item                   | Details                                            |
| ---------------------- | -------------------------------------------------- |
| Project Name           | E-Commerce Web Application – End-to-End QA Testing |
| Application Under Test | Automation Exercise                                |
| Application URL        | https://www.automationexercise.com/                |
| Document Type          | Test Plan                                          |
| Testing Role           | QA Engineer                                        |
| Automation Tool        | Cypress                                            |
| Programming Language   | JavaScript                                         |
| API Testing            | Postman / Cypress                                  |
| Performance Testing    | Apache JMeter                                      |
| Version                | 1.0                                                |

---

## 2. Introduction

This Test Plan defines the testing approach, scope, objectives, resources, and deliverables for testing the Automation Exercise e-commerce web application.

The purpose of this project is to evaluate the application's functionality, usability, reliability, and overall behavior through a combination of manual testing, exploratory testing, UI automation, API testing, and performance testing.

The testing activities will focus on important user journeys such as user registration, login, product search, product selection, shopping cart management, checkout, and other core e-commerce functionality.

---

## 3. Test Objectives

The main objectives of testing are:

* Verify that the application's major features work according to their expected behavior.
* Identify functional defects and unexpected system behavior.
* Validate important end-to-end user journeys.
* Verify positive and negative scenarios.
* Ensure that previously identified defects do not reappear during regression testing.
* Automate selected high-value test scenarios using Cypress.
* Validate available API endpoints using Postman and Cypress.
* Perform basic performance testing using Apache JMeter.
* Document defects using clear and reproducible bug reports.
* Produce professional test documentation and execution reports.

---

## 4. Scope of Testing

### 4.1 In Scope

The following areas will be included in testing:

#### User Management

* User registration
* User login
* Invalid login
* Logout
* User account information
* Account deletion

#### Product Management

* View products
* Product details
* Product search
* Product categories
* Product brands
* Product availability

#### Shopping Cart

* Add products to cart
* Remove products from cart
* Update cart quantities
* Verify cart details
* Verify product prices and totals

#### Checkout

* Proceed to checkout
* Verify delivery details
* Verify billing information
* Place an order
* Order confirmation

#### Other Features

* Home page
* Navigation
* Contact Us
* Subscription functionality
* Responsive and cross-browser behavior where applicable

#### API

* Available product APIs
* User-related APIs
* Brand/category APIs
* Cart/order-related APIs where available

#### Performance

* Basic load testing of selected application endpoints/pages
* Response time observation
* Behavior under concurrent requests

---

## 5. Out of Scope

The following areas are outside the primary scope of this portfolio project:

* Real financial transactions using actual payment information
* Production infrastructure testing
* Server-level security penetration testing
* Database-level testing
* Source-code unit testing
* Extensive mobile application testing
* Destructive stress testing of the public application
* Testing of third-party systems outside the application's control

---

## 6. Testing Approach

A combination of testing techniques will be used throughout the project.

### 6.1 Manual Testing

Manual testing will be used to validate application functionality and user workflows.

Activities include:

* Test scenario creation
* Detailed test case design
* Positive testing
* Negative testing
* Boundary testing where applicable
* UI validation
* Usability checks
* Regression testing

### 6.2 Exploratory Testing

Exploratory testing will be performed to discover unexpected behavior that may not be identified through predefined test cases.

Exploratory testing will focus on:

* Navigation
* Input validation
* User interactions
* Cart behavior
* Error handling
* Unexpected input combinations
* UI inconsistencies

### 6.3 UI Automation

Cypress will be used to automate selected high-priority and repetitive test scenarios.

The automation suite will focus on:

* Authentication
* Product search
* Product selection
* Cart functionality
* Checkout workflows
* Regression scenarios

Automation will include appropriate assertions, reusable commands, test organization, screenshots, and test reporting.

### 6.4 API Testing

API testing will be performed using Postman and Cypress.

Testing will include:

* HTTP methods
* Status codes
* Response body validation
* Request parameters
* Response structure
* Positive and negative API scenarios

### 6.5 Performance Testing

Apache JMeter will be used to perform basic performance testing of selected application endpoints.

The performance testing will examine:

* Response time
* Throughput
* Error rate
* Behavior under controlled concurrent requests

Performance tests will be conducted responsibly against the available demo environment.

---

## 7. Test Levels

The following testing levels will be considered:

### Functional Testing

Verify that application features behave according to their expected functionality.

### Integration/API Testing

Verify communication between application components through available APIs.

### System Testing

Validate complete user workflows across the application.

### Regression Testing

Verify that changes or fixes do not negatively affect existing functionality.

---

## 8. Test Types

The project will include:

| Test Type             | Purpose                                               |
| --------------------- | ----------------------------------------------------- |
| Functional Testing    | Verify application functionality                      |
| Smoke Testing         | Verify critical functionality before detailed testing |
| Regression Testing    | Verify existing functionality after changes/fixes     |
| Exploratory Testing   | Discover unexpected defects                           |
| UI Testing            | Validate interface and user interactions              |
| Usability Testing     | Identify usability issues                             |
| Cross-Browser Testing | Verify behavior across supported browsers             |
| Automation Testing    | Automate repeatable regression scenarios              |
| API Testing           | Validate API behavior and responses                   |
| Performance Testing   | Evaluate response and behavior under load             |

---

## 9. Test Environment

### Application

**Automation Exercise**

https://www.automationexercise.com/

### Primary Browser

* Google Chrome

### Additional Browsers

Where applicable:

* Microsoft Edge
* Mozilla Firefox

### Operating System

* Windows

### Automation Environment

* Cypress
* JavaScript
* Node.js

### API Testing Environment

* Postman
* Cypress API testing

### Performance Testing Environment

* Apache JMeter

### Version Control

* Git
* GitHub

---

## 10. Test Data

Test data will be created specifically for the testing activities.

Examples include:

* Valid user registration details
* Invalid email addresses
* Invalid passwords
* Existing user credentials where permitted
* Product search keywords
* Valid and invalid input values
* Cart quantities
* Checkout information

Sensitive personal or financial information will not be used.

---

## 11. Defect Management

Identified defects will be documented using structured bug reports.

Each defect report will include:

* Bug ID
* Bug Title
* Description
* Preconditions
* Steps to Reproduce
* Expected Result
* Actual Result
* Severity
* Priority
* Environment
* Evidence/Screenshot
* Status

Defects will be categorized according to their impact and urgency.

---

## 12. Severity and Priority

### Severity

Severity represents the impact of a defect on the application.

* **Critical** – Prevents a major part of the system from functioning.
* **High** – Major functionality is significantly affected.
* **Medium** – Functionality is affected but a workaround may exist.
* **Low** – Minor functional or UI issue.

### Priority

Priority represents how urgently a defect should be addressed.

* **High** – Requires immediate attention.
* **Medium** – Should be addressed in the normal development cycle.
* **Low** – Can be addressed later.

Severity and priority will be assigned independently based on the characteristics of each defect.

---

## 13. Entry Criteria

Testing will begin when:

* The application is accessible.
* The major application features can be accessed.
* Basic application requirements have been identified.
* The test environment is available.
* Required testing tools are configured.

---

## 14. Exit Criteria

Testing activities will be considered complete when:

* Planned test cases have been executed.
* Critical user journeys have been tested.
* Identified defects have been documented.
* Critical issues identified during testing have been retested where possible.
* Selected automation scenarios have been implemented and executed.
* Planned API tests have been completed.
* Planned performance tests have been completed.
* Test results have been documented.
* A final QA summary has been prepared.

---

## 15. Deliverables

The project will produce the following deliverables:

1. Application Overview
2. Test Plan
3. Test Scenarios
4. Test Cases
5. Exploratory Testing Notes
6. Bug Reports
7. Cypress Automation Scripts
8. API Test Collection and Results
9. JMeter Performance Test Plan
10. Test Execution Results
11. Final QA Test Report

---

## 16. Risks and Mitigation

| Risk                                                    | Mitigation                                                                    |
| ------------------------------------------------------- | ----------------------------------------------------------------------------- |
| Demo application changes during testing                 | Document observed behavior and update test cases when required                |
| Application becomes temporarily unavailable             | Retry testing later and record environment availability                       |
| Test data becomes invalid                               | Create controlled test data where possible                                    |
| Automation scripts become unstable due to UI changes    | Use reliable selectors and reusable Cypress commands                          |
| Performance testing affects the public demo environment | Use controlled and limited load levels                                        |
| Third-party services behave differently                 | Document limitations and separate third-party issues from application defects |

---

## 17. Roles and Responsibilities

### QA Engineer

Responsibilities include:

* Analyze application functionality
* Design test scenarios
* Create test cases
* Execute manual tests
* Perform exploratory testing
* Report defects
* Develop Cypress automation tests
* Perform API testing
* Execute performance tests
* Prepare test reports
* Maintain QA documentation

---

## 18. Test Execution Strategy

Testing will be performed progressively:

**Phase 1 – Application Understanding**

Understand the application structure, features, and major user journeys.

**Phase 2 – Manual Testing**

Create and execute test scenarios and detailed test cases.

**Phase 3 – Exploratory Testing**

Explore the application to identify unexpected behavior and usability issues.

**Phase 4 – Defect Management**

Document discovered defects and perform retesting where applicable.

**Phase 5 – Automation**

Automate selected high-value regression scenarios using Cypress.

**Phase 6 – API Testing**

Validate available APIs using Postman and Cypress.

**Phase 7 – Performance Testing**

Perform controlled performance testing using Apache JMeter.

**Phase 8 – Final Reporting**

Analyze results and prepare the final QA report.

---

## 19. Success Criteria

The project will be considered successful when the planned testing activities have been completed and the results provide sufficient evidence about the application's functional behavior, identified defects, automation coverage, API behavior, and basic performance characteristics.

---

## 20. Document Version History

| Version | Date       | Description       |
| ------- | ---------- | ----------------- |
| 1.0     | 2026-09-26 | Initial Test Plan |
