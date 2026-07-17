# Definition

**Equivalence Partitioning** is a software testing technique in which input data is divided into valid and invalid partitions, and one value from each partition is selected for testing.

---

# Why Use Equivalence Partitioning?

- Reduces the number of test cases.
- Saves testing time and effort.
- Improves test coverage.
- Eliminates redundant test cases.
- Helps identify defects efficiently.
- Simplifies test design.

---

# Objective of Equivalence Partitioning

- Divide input values into logical groups.
- Test one representative value from each group.
- Ensure complete functional validation.
- Reduce duplicate testing.

---

# Types of Equivalence Partitioning

## 1. Valid Equivalence Partition

Contains input values that should be **accepted** by the application.

### Example

Age should be between **18 and 60**.

Valid Partition:

```text
18 – 60
```

Representative Value:

```text
25
```

---

## 2. Invalid Equivalence Partition

Contains input values that should be **rejected** by the application.

### Example

Age should be between **18 and 60**.

Invalid Partitions:

```text
Less than 18

Greater than 60
```

Representative Values:

```text
15

65
```

---

# Equivalence Partitioning Workflow

```text
Requirement
      │
      ▼
Identify Input Field
      │
      ▼
Divide into Partitions
      │
      ▼
Select Representative Value
      │
      ▼
Design Test Cases
      │
      ▼
Execute Test Cases
```

---

# Real-Time Example 1 – Age Validation

### Requirement

User age should be between **18 and 60**.

| Partition | Type | Test Value | Expected Result |
|------------|------|------------|-----------------|
| Less than 18 | Invalid | 15 | Reject |
| 18–60 | Valid | 30 | Accept |
| Greater than 60 | Invalid | 65 | Reject |

---
# Real-Time Example 2 – Password Length

### Requirement

Password should contain **8 to 16 characters**.

| Partition | Type | Test Value | Expected Result |
|------------|------|------------|-----------------|
| Less than 8 | Invalid | 6 Characters | Reject |
| 8–16 | Valid | 10 Characters | Accept |
| Greater than 16 | Invalid | 18 Characters | Reject |

---

# Real-Time Example 3 – Marks Validation

### Requirement

Marks should be between **0 and 100**.

| Partition | Type | Test Value | Expected Result |
|------------|------|------------|-----------------|
| Less than 0 | Invalid | -5 | Reject |
| 0–100 | Valid | 75 | Accept |
| Greater than 100 | Invalid | 120 | Reject |

---

# Real-Time Example 4 – OrangeHRM Login

### Requirement

Username and Password are mandatory.

### Username

| Partition | Type | Example |
|------------|------|---------|
| Valid Username | Valid | Admin |
| Invalid Username | Invalid | Admin12345 |
| Blank Username | Invalid | "" |

### Password

| Partition | Type | Example |
|------------|------|---------|
| Valid Password | Valid | admin123 |
| Invalid Password | Invalid | password123 |
| Blank Password | Invalid | "" |

---

# Steps to Apply Equivalence Partitioning

1. Understand the requirement.
2. Identify the input field.
3. Divide inputs into valid and invalid partitions.
4. Select one representative value from each partition.
5. Design test cases.
6. Execute and verify results.

---

# Advantages

- Reduces the number of test cases.
- Improves testing efficiency.
- Covers both valid and invalid inputs.
- Saves execution time.
- Easy to understand and implement.
- Avoids repetitive testing.

---

# Disadvantages

- Not suitable for complex business logic.
- May miss defects at boundary values.
- Works best with clearly defined input ranges.
- Should be combined with Boundary Value Analysis (BVA).

---

# Equivalence Partitioning vs Boundary Value Analysis

| Equivalence Partitioning | Boundary Value Analysis |
|--------------------------|-------------------------|
| Divides inputs into partitions. | Tests values at the boundaries. |
| One value from each partition is tested. | Boundary values are tested. |
| Reduces the number of test cases. | Focuses on edge cases. |
| Covers valid and invalid partitions. | Covers minimum and maximum limits. |

---

# Best Practices

- Identify all valid and invalid partitions.
- Choose only one representative value from each partition.
- Combine EP with Boundary Value Analysis.
- Ensure every partition is covered.
- Review test cases before execution.

---

# Common Mistakes

- Ignoring invalid partitions.
- Selecting multiple values from the same partition unnecessarily.
- Missing a valid partition.
- Using only valid inputs.
- Confusing EP with Boundary Value Analysis.

---

# Key Learnings

- Equivalence Partitioning is a Black Box Testing technique.
- It divides input data into valid and invalid partitions.
- One representative value is selected from each partition.
- It reduces the number of test cases while maintaining good coverage.
- It is often used together with Boundary Value Analysis for effective testing.

---


# Interview Questions

### Q1. What is Equivalence Partitioning?

---

### Q2. Why is Equivalence Partitioning used?

---

### Q3. What are the types of Equivalence Partitioning?

---

### Q4. What is a Representative Value?

---

### Q5. What is the difference between Equivalence Partitioning and Boundary Value Analysis?

---

### Q6. Give a real-time example of Equivalence Partitioning.

---

# Summary

- **Equivalence Partitioning (EP)** is a **Black Box Testing** technique.
- Input data is divided into **Valid** and **Invalid** partitions.
- One representative value is selected from each partition.
- EP reduces the number of test cases while maintaining effective coverage.
- It is commonly used with **Boundary Value Analysis (BVA)** for better defect detection.
