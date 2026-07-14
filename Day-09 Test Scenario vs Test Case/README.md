# Day 09 – Test Scenario vs Test Case

## What is a Test Scenario?

A **Test Scenario** is a high-level statement that describes **what needs to be tested** in an application. It represents a functionality or feature that should be verified without going into detailed test steps.

A Test Scenario helps ensure that all business requirements are covered during testing.

### Example

**Module:** Login

**Test Scenario:** Verify Login Functionality

---

# What is a Test Case?

A **Test Case** is a detailed document that explains **how to test** a particular functionality. It includes preconditions, test steps, test data, expected results, and actual results.

Test cases are executed by testers to validate whether the application behaves as expected.

### Example

**Test Case:** Verify login with valid username and password.

- Enter valid username.
- Enter valid password.
- Click Login.
- Verify that the Dashboard page is displayed.

---

# Difference Between Test Scenario and Test Case

| Test Scenario | Test Case |
|---------------|-----------|
| High-level description of what to test. | Detailed document describing how to test. |
| Covers a feature or functionality. | Covers specific conditions of a feature. |
| Derived from business requirements. | Derived from test scenarios and requirements. |
| Contains minimal details. | Contains complete execution steps. |
| Helps identify testing scope. | Helps validate application behavior. |
| One scenario can have multiple test cases. | Each test case validates one specific condition. |

---

# Components of a Test Scenario

A Test Scenario generally includes:

- Scenario ID
- Module Name
- Test Scenario Description
- Requirement Reference
- Priority

---

# Components of a Test Case

A standard Test Case contains:

- Test Case ID
- Test Scenario
- Module
- Precondition
- Test Steps
- Test Data
- Expected Result
- Actual Result
- Status
- Priority
- Remarks

---

# Relationship Between Test Scenario and Test Case

```text
Requirement
      │
      ▼
Test Scenario
      │
      ▼
Test Cases
      │
      ▼
Test Execution
      │
      ▼
Defect Reporting
```

---

# Real-Time Example (OrangeHRM Login)

### Test Scenario

**Verify Login Functionality**

### Test Cases

- Login with valid credentials.
- Login with invalid username.
- Login with invalid password.
- Login with blank username.
- Login with blank password.
- Login with both fields blank.
- Verify password is case-sensitive.
- Verify SQL Injection attempt.
- Verify session timeout.
- Verify logout functionality.

---

# Real-Time Example (Amount Transfer)

### Test Scenario

**Verify Amount Transfer Functionality**

### Test Cases

- Transfer amount with valid account details.
- Transfer with invalid From Account Number.
- Transfer with invalid To Account Number.
- Transfer with insufficient balance.
- Transfer with zero amount.
- Transfer with negative amount.
- Transfer without entering mandatory fields.
- Verify maximum amount limit.
- Verify minimum amount limit.
- Verify Cancel button functionality.

---

# Characteristics of a Good Test Scenario

A good Test Scenario should:

- Be simple and easy to understand.
- Cover business requirements.
- Be independent.
- Cover both positive and negative flows.
- Be reusable whenever possible.

---

# Characteristics of a Good Test Case

A good Test Case should:

- Be clear and concise.
- Have unique Test Case ID.
- Include proper preconditions.
- Contain detailed execution steps.
- Mention expected results clearly.
- Be reusable.
- Be easy to maintain.
- Cover positive, negative, and boundary conditions.

---

# Advantages of Test Scenarios

- Easy to prepare.
- Ensures complete requirement coverage.
- Helps estimate testing effort.
- Simplifies test planning.
- Provides high-level visibility.

---

# Advantages of Test Cases

- Ensures detailed validation.
- Improves test coverage.
- Makes defect identification easier.
- Helps during regression testing.
- Can be reused in future releases.

---

# Test Scenario vs Test Case Workflow

```text
Business Requirement
         │
         ▼
Requirement Analysis
         │
         ▼
Prepare Test Scenarios
         │
         ▼
Design Test Cases
         │
         ▼
Review Test Cases
         │
         ▼
Execute Test Cases
         │
         ▼
Report Defects
```

---

# Best Practices

- Understand requirements before writing scenarios.
- Write one scenario for each functionality.
- Design multiple test cases for every scenario.
- Cover positive, negative, boundary, and validation cases.
- Keep test cases independent.
- Review test cases before execution.
- Maintain traceability with requirements.

---

# Common Mistakes

- Confusing Test Scenario with Test Case.
- Missing negative test cases.
- Writing unclear expected results.
- Skipping boundary value testing.
- Creating duplicate test cases.
- Not updating test cases after requirement changes.

---

# Key Learnings

- Test Scenarios describe **what to test**.
- Test Cases describe **how to test**.
- One Test Scenario can have multiple Test Cases.
- Test Cases provide detailed execution instructions.
- Proper Test Scenario and Test Case design improves software quality and test coverage.

---

# Interview Questions

### Q1. What is a Test Scenario?

---

### Q2. What is a Test Case?

---

### Q3. What is the difference between a Test Scenario and a Test Case?

---

### Q4. Can one Test Scenario have multiple Test Cases?

---

### Q5. Why are Test Cases important?

---

### Q6. Which is created first: Test Scenario or Test Case?

---

# Summary

- **Test Scenario = What to Test**
- **Test Case = How to Test**
- Test Scenarios provide high-level coverage.
- Test Cases provide detailed execution steps.
- Both are essential for effective software testing and quality assurance.
