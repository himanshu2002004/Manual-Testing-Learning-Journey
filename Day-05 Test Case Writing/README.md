# Day 5 – Test Case Writing

## What is a Test Case?

A Test Case is a document that describes:

* What needs to be tested
* How it should be tested
* Expected outcome
* Actual outcome
* Test status

In simple words it is a well-written test case helps testers execute tests consistently, identify defects efficiently, and ensure complete requirement coverage.

---

# Why are Test Cases Important?

* Ensures complete requirement coverage.
* Provides a structured testing approach.
* Improves testing consistency.
* Helps identify defects.
* Reduces duplicate testing.
* Supports regression testing.
* Acts as project documentation.
* Improves communication among team members.

---

# Objectives of Test Case Writing

* Verify application functionality.
* Validate business requirements.
* Detect defects.
* Improve software quality.
* Maintain testing documentation.
* Enable repeatable testing.

---

# Characteristics of a Good Test Case

A good test case should be:

* Clear
* Simple
* Easy to understand
* Reusable
* Independent
* Traceable
* Maintainable
* Accurate
* Complete

---

# Components of a Test Case

A standard test case usually contains:

* Test Case ID
* Module Name
* Test Scenario
* Test Case Description
* Preconditions
* Test Steps
* Test Data
* Expected Result
* Actual Result
* Status
* Priority
* Severity
* Author
* Execution Date
* Comments

---

# Test Case Template

| Field           | Description                    |
| --------------- | ------------------------------ |
| Test Case ID    | Unique identifier              |
| Module          | Module under test              |
| Test Scenario   | High-level functionality       |
| Test Case       | Detailed verification          |
| Preconditions   | Conditions before execution    |
| Test Steps      | Execution steps                |
| Test Data       | Input data                     |
| Expected Result | Expected behavior              |
| Actual Result   | Actual behavior                |
| Status          | Pass / Fail                    |
| Priority        | High / Medium / Low            |
| Severity        | Critical / High / Medium / Low |
| Remarks         | Additional comments            |

---

# Test Case Design Process

```text
Requirement
      ↓
Understand Requirement
      ↓
Identify Test Scenarios
      ↓
Prepare Test Cases
      ↓
Review Test Cases
      ↓
Execute Test Cases
      ↓
Report Defects
      ↓
Update Test Cases
```

---

# Types of Test Cases

## Positive Test Case

Verifies the application behaves correctly with valid inputs.

Example:

Username: Admin

Password: admin123

Expected Result:

Login Successful

---

## Negative Test Case

Verifies application behavior using invalid inputs.

Example:

Wrong Password

Expected Result:

Invalid credentials message displayed.

---

## Boundary Value Test Case

Tests minimum and maximum input values.

Example:

Password

Minimum Length : 8

Maximum Length :10

---

## Validation Test Case

Checks mandatory field validations.

Example

Leave username blank.

Expected Result

Username is required.

---

## Error Handling Test Case

Verifies appropriate error messages.

Example

Invalid Email Format

Expected Result

Please enter a valid email.

---

## End-to-End Test Case

Verifies complete business workflow.

Example

```text
Login

  ↓

Search Product

  ↓

Add to Cart

  ↓

Checkout

  ↓

Payment

  ↓

Logout

```

---

# Example Test Case

Module

Login

Test Scenario

Verify Login Functionality

Test Case ID

TC_LOG_001

Precondition

Application is accessible.

Steps

1. Open OrangeHRM.
2. Enter valid Username.
3. Enter valid Password.
4. Click Login.

Expected Result

Dashboard should open successfully.

Actual Result

Dashboard opened successfully.

Status

Pass

---

# Best Practices

* Use unique Test Case IDs.
* Keep test cases simple.
* Write one verification per test case.
* Use clear expected results.
* Avoid ambiguous language.
* Include positive and negative scenarios.
* Review test cases before execution.
* Update test cases when requirements change.

---

# Common Mistakes

* Missing expected results.
* Combining multiple validations in one test case.
* Unclear steps.
* Duplicate test cases.
* Missing preconditions.
* Poor naming convention.
* No requirement mapping.

---

# Test Case vs Test Scenario

| Test Scenario            | Test Case                    |
| ------------------------ | ---------------------------- |
| High-level functionality | Detailed verification        |
| Covers feature           | Covers individual conditions |
| Few in number            | Many for each scenario       |
| Requirement-focused      | Execution-focused            |

---

# Real-Time Example (OrangeHRM Login)

Scenario

Verify Login

Test Cases

* Valid Login
* Invalid Password
* Invalid Username
* Blank Username
* Blank Password
* Blank Username and Password
* Password Case Sensitivity
* SQL Injection Attempt
* Session Timeout
* Logout Verification

---

# Deliverables

* Test Case Document
* Test Execution Report
* Defect Report
* Requirement Traceability Matrix

---

# Key Learnings

* Test cases provide a structured way to validate application functionality.
* Every requirement should have corresponding test cases.
* Well-written test cases improve testing quality and maintainability.
* Good test cases help identify defects early and support regression testing.

---

# Interview Questions

### Q1. What is a Test Case?

---

### Q2. What is the difference between a Test Scenario and a Test Case?

---

### Q3. What are the components of a Test Case?

---

### Q4. What is the difference between Priority and Severity?

---

### Q5. What are Positive and Negative Test Cases?

---

### Q6. What are the characteristics of a good Test Case?

---
