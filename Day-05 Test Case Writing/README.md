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

Test Scenario

Verify Amount Transfer Functionality

Test Case ID

TC_TRANS_001

Precondition
* User is logged into the application.
* User has sufficient account balance.
* Both source and destination accounts are valid.
Test Steps
* Navigate to the Fund Transfer page.
* Enter a valid From Account Number.
* Enter a valid To Account Number.
* Enter a valid transfer amount.
* Click the Transfer button.
Test Data
* Field	Value
* From Account	12345678
* To Account	87654321
* Amount	5000
  
Expected Result
The amount should be transferred successfully, a success message should be displayed, and the updated account balance should be reflected.

Actual Result
Amount transferred successfully and confirmation message displayed.

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

# Test Cases
* Verify successful amount transfer using valid From Account, To Account, and Amount.
* Verify transfer with an invalid From Account Number.
* Verify transfer with an invalid To Account Number.
* Verify transfer when From Account Number is left blank.
* Verify transfer when To Account Number is left blank.
* Verify transfer when the Amount field is left blank.
* Verify transfer when all fields are left blank.
* Verify transfer with an amount greater than the available account balance.
* Verify transfer with an amount equal to the available account balance.
* Verify transfer with the minimum allowed amount.
* Verify transfer with the maximum allowed amount.
* Verify transfer with zero amount.
* Verify transfer with a negative amount.
* Verify transfer with decimal values (if supported).
* Verify transfer with special characters entered in the account number fields.
* Verify transfer with alphabetic characters entered in the account number fields.
* Verify transfer when the From Account Number and To Account Number are the same.
* Verify transfer with an account number having fewer than the minimum required digits.
* Verify transfer with an account number exceeding the maximum allowed digits.
* Verify successful transfer using valid minimum-length account numbers.
* Verify successful transfer using valid maximum-length account numbers.
* Verify the Transfer button is enabled only when all mandatory fields contain valid data.
* Verify the Cancel button cancels the transaction.
* Verify the Cancel button redirects to the previous page or dashboard (as per application design).

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
