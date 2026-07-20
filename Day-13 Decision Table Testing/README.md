# Day 13 – Decision Table Testing

## What is Decision Table Testing?

**Decision Table Testing (DTT)** is a **Black Box Testing** technique used to test applications where the output depends on **multiple input conditions**. It helps testers identify all possible combinations of conditions and their corresponding actions in a structured table format.

Decision Table Testing is especially useful for validating **business rules**, **complex logic**, and **decision-based workflows**.

---

# Why Use Decision Table Testing?

- Ensures all possible condition combinations are tested.
- Simplifies testing of complex business logic.
- Reduces the chances of missing test scenarios.
- Improves test coverage.
- Makes test case design more systematic and organized.
- Helps identify inconsistencies in business requirements.

---

# Objective of Decision Table Testing

- Verify business rules.
- Test multiple input combinations.
- Reduce redundant test cases.
- Ensure accurate application behavior for every possible condition.

---

# Components of a Decision Table

A Decision Table consists of four main parts:

### 1. Conditions

Input values or criteria that affect the application's behavior.

### 2. Condition Alternatives

Possible values for each condition (Yes/No, True/False, etc.).

### 3. Actions

Expected outputs or actions performed by the application.

### 4. Action Entries

Indicates whether an action should occur for a particular combination of conditions.

---

# Structure of a Decision Table

| Conditions / Actions | Rule 1 | Rule 2 | Rule 3 | Rule 4 |
|----------------------|--------|--------|--------|--------|
| Condition 1 | Yes | Yes | No | No |
| Condition 2 | Yes | No | Yes | No |
| Action | Perform Action | Perform Action | Perform Action | Reject |

---

# Decision Table Workflow

```text
Requirement
      │
      ▼
Identify Conditions
      │
      ▼
Identify Possible Values
      │
      ▼
Create Decision Table
      │
      ▼
Generate Test Cases
      │
      ▼
Execute Test Cases
```

---

# Real-Time Example 1 – ATM Withdrawal

### Requirement

A customer can withdraw money only if:

- Card is valid.
- Sufficient balance is available.

| Card Valid | Sufficient Balance | Expected Result |
|-------------|--------------------|-----------------|
| Yes | Yes | Cash Dispensed |
| Yes | No | Insufficient Balance |
| No | Yes | Invalid Card |
| No | No | Invalid Card |

---

# Real-Time Example 2 – Login Functionality

### Requirement

User can log in only if:

- Username is valid.
- Password is valid.

| Username Valid | Password Valid | Expected Result |
|----------------|----------------|-----------------|
| Yes | Yes | Login Successful |
| Yes | No | Invalid Password |
| No | Yes | Invalid Username |
| No | No | Invalid Credentials |

---

# Real-Time Example 3 – E-Commerce Discount

### Requirement

A customer receives a **10% discount** only if:

- Customer is a Premium Member.
- Order Amount is greater than ₹5000.

| Premium Member | Order > ₹5000 | Expected Result |
|----------------|---------------|-----------------|
| Yes | Yes | Discount Applied |
| Yes | No | No Discount |
| No | Yes | No Discount |
| No | No | No Discount |

---

# Real-Time Example 4 – OrangeHRM Login

### Requirement

The user can log in only if:

- Username is correct.
- Password is correct.
- User account is active.

| Username | Password | Account Active | Expected Result |
|----------|----------|----------------|-----------------|
| Correct | Correct | Yes | Login Successful |
| Correct | Correct | No | Account Disabled |
| Correct | Incorrect | Yes | Invalid Password |
| Incorrect | Correct | Yes | Invalid Username |
| Incorrect | Incorrect | No | Login Failed |

---

# Steps to Apply Decision Table Testing

1. Understand the business requirement.
2. Identify all input conditions.
3. Determine possible values for each condition.
4. List all possible combinations.
5. Define expected actions.
6. Create the decision table.
7. Design test cases.
8. Execute and verify results.

---

# Advantages

- Covers all possible input combinations.
- Ideal for business rule validation.
- Reduces missing test scenarios.
- Improves requirement understanding.
- Easy to maintain and review.
- Helps identify ambiguous requirements.

---

# Disadvantages

- Decision tables become large as the number of conditions increases.
- Time-consuming for highly complex systems.
- Not suitable for simple input validation.
- Requires clear business rules.

---

# Decision Table Testing vs Equivalence Partitioning

| Decision Table Testing | Equivalence Partitioning |
|------------------------|--------------------------|
| Tests combinations of conditions. | Tests representative values from partitions. |
| Suitable for business rules. | Suitable for input validation. |
| Uses conditions and actions. | Uses valid and invalid partitions. |
| Focuses on decision logic. | Focuses on input ranges. |

---

# Decision Table Testing vs Boundary Value Analysis

| Decision Table Testing | Boundary Value Analysis |
|------------------------|-------------------------|
| Tests combinations of conditions. | Tests boundary values. |
| Used for business logic. | Used for numeric or range-based inputs. |
| Covers decision rules. | Covers edge cases. |

---

# Best Practices

- Clearly identify all business rules.
- Include every possible combination of conditions.
- Remove duplicate combinations if applicable.
- Review the decision table with stakeholders.
- Keep the table simple and easy to understand.

---

# Common Mistakes

- Missing condition combinations.
- Incorrect expected actions.
- Ignoring exceptional cases.
- Creating duplicate rules.
- Misinterpreting business requirements.

---

# Key Learnings

- Decision Table Testing is a Black Box Testing technique.
- It is used when application behavior depends on multiple conditions.
- Decision tables help organize business rules clearly.
- Every combination of conditions should be validated.
- It improves test coverage and reduces missed scenarios.

---

# Interview Questions

### Q1. What is Decision Table Testing?

---

### Q2. When should Decision Table Testing be used?

---

### Q3. What are the components of a Decision Table?

---

### Q4. What are the advantages of Decision Table Testing?

---

### Q5. What is the difference between Decision Table Testing and Boundary Value Analysis?

---

### Q6. Give a real-time example of Decision Table Testing.

---
