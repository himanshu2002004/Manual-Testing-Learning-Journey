# Day 10 – Requirement Traceability Matrix (RTM)
---

# Definition

**Requirement Traceability Matrix (RTM)** is a document that maps project requirements with their corresponding test scenarios, test cases, execution status, and defects to ensure complete requirement coverage.

---

# Why is RTM Important?

RTM plays a crucial role in software testing because it helps ensure that all requirements are tested throughout the Software Testing Life Cycle (STLC).

### Benefits

- Ensures 100% requirement coverage.
- Verifies that no requirement is missed.
- Helps identify missing test cases.
- Improves test coverage.
- Makes defect tracking easier.
- Supports change impact analysis.
- Helps during regression testing.
- Improves project quality.
- Acts as proof that all requirements have been tested.

---

# Objectives of RTM

- Track requirements throughout the project.
- Ensure every requirement has at least one test case.
- Maintain traceability between requirements and testing artifacts.
- Identify missing requirements or test cases.
- Support defect management.
- Improve software quality.

---

# Requirement Traceability Flow

```text
Business Requirement
          │
          ▼
Software Requirement Specification (SRS)
          │
          ▼
    Test Scenario
          │
          ▼
      Test Case
          │
          ▼
    Test Execution
          │
          ▼
    Defect Report
          │
          ▼
     Test Closure
```

---

# Types of Requirement Traceability

## 1. Forward Traceability

Forward Traceability ensures that **every requirement is covered by one or more test cases.**

```text
Requirement
  │
  ▼
Test Case
```

**Purpose**

- Ensure complete requirement coverage.
- Prevent missing functionalities.

---

## 2. Backward (Reverse) Traceability

Backward Traceability ensures that **every test case is linked back to a valid requirement.**

```text
Test Case
  │
  ▼
Requirement
```

**Purpose**

- Avoid unnecessary test cases.
- Ensure every test case has a business purpose.

---

## 3. Bidirectional Traceability

Bidirectional Traceability combines both Forward and Backward Traceability.

```text
Requirement
      ↕
Test Case
```

**Purpose**

- Complete traceability.
- Easier impact analysis.
- Better change management.

---

# Components of RTM

A standard RTM contains the following fields:

- Requirement ID
- Requirement Description
- Module
- Test Scenario ID
- Test Case ID
- Test Case Description
- Priority
- Test Status
- Defect ID
- Remarks

---

# RTM Template

| Requirement ID | Requirement Description | Module | Test Scenario ID | Test Case ID | Test Status | Defect ID |
|----------------|-------------------------|--------|------------------|--------------|-------------|------------|
| REQ_001 | User Login | Login | TS_LOG_001 | TC_LOG_001 | Pass | - |
| REQ_002 | Invalid Login | Login | TS_LOG_002 | TC_LOG_002 | Fail | BUG_001 |

---

# Example RTM (OrangeHRM Login Module)

| Requirement ID | Requirement | Test Scenario | Test Case | Status | Defect |
|----------------|-------------|--------------|-----------|--------|---------|
| REQ_LOG_001 | User should login with valid credentials | Verify Login | TC_LOG_001 | Pass | - |
| REQ_LOG_002 | Display error for invalid password | Verify Invalid Login | TC_LOG_002 | Pass | - |
| REQ_LOG_003 | Validate mandatory fields | Verify Blank Login | TC_LOG_003 | Pass | - |
| REQ_LOG_004 | Logout successfully | Verify Logout | TC_LOG_004 | Pass | - |

---

# Example RTM (Amount Transfer Module)

| Requirement ID | Requirement | Test Scenario | Test Case | Status | Defect |
|----------------|-------------|--------------|-----------|--------|---------|
| REQ_TRN_001 | Transfer amount successfully | Verify Fund Transfer | TC_TRN_001 | Pass | - |
| REQ_TRN_002 | Validate account number | Verify Account Validation | TC_TRN_002 | Pass | - |
| REQ_TRN_003 | Validate transfer amount | Verify Amount Validation | TC_TRN_003 | Pass | - |
| REQ_TRN_004 | Cancel transaction | Verify Cancel Functionality | TC_TRN_004 | Pass | - |

---

# Advantages of RTM

- Ensures complete requirement coverage.
- Improves traceability.
- Identifies missing test cases.
- Simplifies defect tracking.
- Supports impact analysis.
- Helps in regression testing.
- Improves project documentation.
- Enhances communication between stakeholders.

---

# Disadvantages of RTM

- Time-consuming to prepare.
- Requires regular updates.
- Difficult to maintain for large projects.
- Can become complex if requirements change frequently.

---

# Best Practices

- Assign unique Requirement IDs.
- Map every requirement to at least one test case.
- Update RTM whenever requirements change.
- Maintain bidirectional traceability.
- Review RTM regularly.
- Link defects with corresponding requirements.

---

# Common Mistakes

- Missing Requirement IDs.
- One requirement not mapped to any test case.
- Duplicate mappings.
- Outdated RTM after requirement changes.
- Incorrect Test Case references.
- Ignoring defect mapping.

---

# RTM Workflow

```text
Requirement Analysis
        │
        ▼
Create Requirement IDs
        │
        ▼
Prepare Test Scenarios
        │
        ▼
  Design Test Cases
        │
        ▼
    Create RTM
        │
        ▼
Execute Test Cases
        │
        ▼
Update Execution Status
        │
        ▼
  Link Defects
        │
        ▼
    Finalize RTM
```

---

# Role of RTM in STLC

RTM is used throughout the Software Testing Life Cycle.

| STLC Phase | RTM Activity |
|------------|--------------|
| Requirement Analysis | Identify and document requirements |
| Test Planning | Define testing scope |
| Test Case Development | Map requirements to test cases |
| Test Execution | Update execution status |
| Defect Reporting | Link defects to requirements |
| Test Closure | Verify complete requirement coverage |

---

# Key Learnings

- RTM ensures complete requirement coverage.
- Every requirement should be linked to one or more test cases.
- RTM helps identify missing requirements and missing test cases.
- It improves traceability, defect management, and regression testing.
- Maintaining an updated RTM improves software quality and project transparency.

---

# Interview Questions

### Q1. What is RTM?

---

### Q2. Why is RTM used?

---

### Q3. What are the types of RTM?

---

### Q4. What is Forward Traceability?

---

### Q5. What is Backward Traceability?

---

### Q6. What are the components of RTM?

---

### Q7. What are the benefits of RTM?

---

# Summary

- **RTM = Requirement Traceability Matrix**
- Maps **Requirements → Test Scenarios → Test Cases → Execution → Defects**
- Ensures **100% Requirement Coverage**
- Improves **Traceability, Test Coverage, and Defect Management**
- Essential document in Manual Testing and Software Quality Assurance.
