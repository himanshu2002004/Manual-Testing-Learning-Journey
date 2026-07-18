# Day 12 – Boundary Value Analysis (BVA)

# Definition

**Boundary Value Analysis (BVA)** is a **Black Box Testing** technique used to test the values at the **boundaries (edges)** of an input range.

It is based on the principle that **defects are more likely to occur at the boundaries of input values than in the middle**.

Instead of testing every possible input value, BVA focuses on the **minimum, maximum, and values just inside and outside the valid range**.

---

# Why Use Boundary Value Analysis?

- Detects defects at input boundaries.
- Reduces the number of test cases.
- Improves test coverage.
- Finds edge-case bugs effectively.
- Saves testing time and effort.

---

# Objective of BVA

- Validate minimum and maximum input values.
- Identify defects occurring at boundaries.
- Improve software reliability.
- Complement Equivalence Partitioning for better coverage.

---

# Principle of Boundary Value Analysis

Most software defects occur at the **edges** of valid input ranges.

For example, if the valid age is **18 to 60**, testers should focus on:

- Just below the minimum
- Minimum value
- Just above the minimum
- Just below the maximum
- Maximum value
- Just above the maximum

---

# Boundary Values

For a valid range of **18–60**, the test values are:

| Boundary | Test Value |
|-----------|------------|
| Minimum - 1 | 17 |
| Minimum | 18 |
| Minimum + 1 | 19 |
| Maximum - 1 | 59 |
| Maximum | 60 |
| Maximum + 1 | 61 |

---

# Real-Time Example 1 – Age Validation

### Requirement

User age should be between **18 and 60**.

| Test Value | Expected Result |
|------------|-----------------|
| 17 | Reject |
| 18 | Accept |
| 19 | Accept |
| 59 | Accept |
| 60 | Accept |
| 61 | Reject |

---

# Real-Time Example 2 – Password Length

### Requirement

Password length should be **8 to 16 characters**.

| Password Length | Expected Result |
|-----------------|-----------------|
| 7 | Reject |
| 8 | Accept |
| 9 | Accept |
| 15 | Accept |
| 16 | Accept |
| 17 | Reject |

---

# Real-Time Example 3 – Marks Validation

### Requirement

Marks should be between **0 and 100**.

| Marks | Expected Result |
|--------|-----------------|
| -1 | Reject |
| 0 | Accept |
| 1 | Accept |
| 99 | Accept |
| 100 | Accept |
| 101 | Reject |

---

# Real-Time Example 4 – ATM Withdrawal

### Requirement

Withdrawal amount should be between **₹100 and ₹10,000**.

| Amount | Expected Result |
|---------|-----------------|
| ₹99 | Reject |
| ₹100 | Accept |
| ₹101 | Accept |
| ₹9,999 | Accept |
| ₹10,000 | Accept |
| ₹10,001 | Reject |

---

# Steps to Apply Boundary Value Analysis

1. Understand the requirement.
2. Identify the valid input range.
3. Determine the minimum and maximum values.
4. Select values:
   - Minimum - 1
   - Minimum
   - Minimum + 1
   - Maximum - 1
   - Maximum
   - Maximum + 1
5. Design test cases.
6. Execute and verify results.

---

# Types of Boundary Value Analysis

## 1. Normal Boundary Value Analysis

Tests only the boundary values within and just outside the valid range.

Example:

Range = **1 to 100**

Test Values:

- 0
- 1
- 2
- 99
- 100
- 101

---

## 2. Robust Boundary Value Analysis

Includes **invalid boundary values** in addition to valid ones to verify how the application handles incorrect inputs.

---

# Advantages

- Finds boundary-related defects effectively.
- Improves software quality.
- Reduces unnecessary test cases.
- Easy to understand and implement.
- Provides excellent edge-case coverage.

---

# Disadvantages

- Applicable mainly to range-based inputs.
- May not detect defects unrelated to boundaries.
- Less effective for complex business logic.
- Should be combined with Equivalence Partitioning.

---

# Boundary Value Analysis vs Equivalence Partitioning

| Boundary Value Analysis | Equivalence Partitioning |
|--------------------------|--------------------------|
| Tests boundary values. | Tests representative values from partitions. |
| Focuses on edge cases. | Focuses on valid and invalid partitions. |
| Detects boundary-related defects. | Reduces the number of test cases. |
| Uses Min-1, Min, Min+1, Max-1, Max, Max+1. | Uses one value from each partition. |

---

# Equivalence Partitioning + BVA Example

### Requirement

Age should be between **18 and 60**.

### Equivalence Partitioning

- 15 → Invalid
- 30 → Valid
- 65 → Invalid

### Boundary Value Analysis

- 17
- 18
- 19
- 59
- 60
- 61

Combining both techniques provides better test coverage.

---

# Best Practices

- Always identify valid input ranges.
- Test both lower and upper boundaries.
- Include values just outside the valid range.
- Combine BVA with Equivalence Partitioning.
- Validate expected results carefully.

---

# Common Mistakes

- Testing only valid boundary values.
- Ignoring invalid boundary values.
- Confusing BVA with Equivalence Partitioning.
- Missing upper or lower boundary tests.
- Not considering business rules.

---

# Key Learnings

- Boundary Value Analysis is a Black Box Testing technique.
- It focuses on testing the boundaries of input ranges.
- Most defects occur at the minimum and maximum limits.
- BVA helps detect edge-case bugs efficiently.
- Combining BVA with Equivalence Partitioning results in more effective test coverage.

---

# Interview Questions

### Q1. What is Boundary Value Analysis (BVA)?

---

### Q2. Why is Boundary Value Analysis used?

---

### Q3. Which values are tested in BVA?

---

### Q4. Give a real-time example of BVA.

---

### Q5. What is the difference between BVA and Equivalence Partitioning?

---

### Q6. Why are BVA and Equivalence Partitioning often used together?

---

# Summary

- **Boundary Value Analysis (BVA)** is a **Black Box Testing** technique.
- It tests values at the **minimum and maximum boundaries** of an input range.
- Standard BVA values are **Min-1, Min, Min+1, Max-1, Max, Max+1**.
- BVA helps detect edge-case defects and improve software quality.
- For the best results, use **Boundary Value Analysis** together with **Equivalence Partitioning**.
