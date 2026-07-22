# Day 14 – State Transition Testing

## What is State Transition Testing?

**State Transition Testing (STT)** is a **Black Box Testing** technique used to verify how a system behaves when it moves from one **state** to another based on specific events or inputs.

A **state** represents the current condition of the system, and a **transition** is the movement from one state to another when an event occurs.

State Transition Testing is commonly used for systems where the output depends on the **current state** as well as the **input**.

---

# Why Use State Transition Testing?

- Validates state-dependent behavior.
- Ensures correct transitions between states.
- Detects invalid state changes.
- Improves test coverage.
- Verifies business workflows.
- Helps identify missing transitions.

---

# Objective of State Transition Testing

- Verify valid state changes.
- Validate invalid transitions.
- Ensure correct system behavior.
- Test business workflows.
- Improve software reliability.

---

# Key Terminologies

## 1. State

A **state** is the current condition of the application.

### Example

For an ATM:

- Idle
- Card Inserted
- PIN Verified
- Transaction Completed

---

## 2. Event

An **event** is an action that causes the application to change its state.

### Example

- Insert Card
- Enter PIN
- Click Login
- Logout

---

## 3. Transition

A **transition** is the movement from one state to another after an event.

Example:

```text
  Idle
   │
Insert Card
   ▼
Card Inserted
```

---

## 4. Initial State

The state where the application starts.

Example:

```
Login Page
```

---

## 5. Final State

The state where the workflow ends.

Example:

```
Logout
```

---

# State Transition Workflow

```text
 Initial State
      │
      ▼
  Event Occurs
      │
      ▼
 State Changes
      │
      ▼
Verify Expected State
```

---

# State Transition Diagram

```text
  Start
   │
   ▼
Login Page
   │
Valid Credentials
   ▼
Dashboard
   │
 Logout
   ▼
Login Page
```

---

# Real-Time Example 1 – Login System

### Requirement

User account gets locked after **3 consecutive invalid login attempts**.

### States

- Login Page
- Login Successful
- Invalid Attempt
- Account Locked

### State Transition Table

| Current State | Event | Next State |
|---------------|-------|------------|
| Login Page | Valid Credentials | Login Successful |
| Login Page | Invalid Password | Invalid Attempt |
| Invalid Attempt | Invalid Password (3rd Attempt) | Account Locked |
| Account Locked | Login Attempt | Access Denied |

---

# Real-Time Example 2 – ATM Machine

### States

- Idle
- Card Inserted
- PIN Verified
- Transaction
- Card Ejected

### State Transition Table

| Current State | Event | Next State |
|---------------|-------|------------|
| Idle | Insert Card | Card Inserted |
| Card Inserted | Enter Correct PIN | PIN Verified |
| PIN Verified | Select Transaction | Transaction |
| Transaction | Finish | Card Ejected |
| Card Ejected | Remove Card | Idle |

---

# Real-Time Example 3 – E-Commerce Order

### States

- Order Placed
- Payment Completed
- Packed
- Shipped
- Delivered
- Cancelled

| Current State | Event | Next State |
|---------------|-------|------------|
| Order Placed | Payment Successful | Payment Completed |
| Payment Completed | Pack Order | Packed |
| Packed | Ship Order | Shipped |
| Shipped | Deliver Order | Delivered |
| Order Placed | Cancel Order | Cancelled |

---

# Real-Time Example 4 – OrangeHRM Login

### States

- Login Page
- Dashboard
- Account Locked
- Logout

| Current State | Event | Next State |
|---------------|-------|------------|
| Login Page | Valid Login | Dashboard |
| Login Page | Invalid Login | Login Page |
| Login Page | 3 Invalid Attempts | Account Locked |
| Dashboard | Logout | Login Page |

---

# Steps to Perform State Transition Testing

1. Understand the business workflow.
2. Identify all possible states.
3. Identify events that trigger transitions.
4. Create a state transition diagram.
5. Prepare a state transition table.
6. Design test cases.
7. Execute test cases.
8. Verify expected transitions.

---

# Advantages

- Ideal for workflow-based applications.
- Detects invalid transitions.
- Improves requirement understanding.
- Ensures complete state coverage.
- Easy to visualize application behavior.
- Useful for login systems, ATM, shopping carts, and workflows.

---

# Disadvantages

- Difficult for highly complex systems.
- Large number of states can make diagrams complex.
- Time-consuming to prepare.
- Not suitable for simple input validation.

---

# State Transition Testing vs Decision Table Testing

| State Transition Testing | Decision Table Testing |
|--------------------------|------------------------|
| Tests state changes. | Tests business rules. |
| Focuses on workflows. | Focuses on input combinations. |
| Uses states and events. | Uses conditions and actions. |
| Best for sequential processes. | Best for decision logic. |

---

# State Transition Testing vs Boundary Value Analysis

| State Transition Testing | Boundary Value Analysis |
|--------------------------|-------------------------|
| Tests state changes. | Tests boundary values. |
| Workflow-based testing. | Range-based testing. |
| Focuses on transitions. | Focuses on edge values. |

---

# Best Practices

- Clearly identify all application states.
- Test both valid and invalid transitions.
- Verify initial and final states.
- Cover every possible state change.
- Review diagrams with stakeholders.
- Update state diagrams when requirements change.

---

# Common Mistakes

- Ignoring invalid transitions.
- Missing intermediate states.
- Not testing repeated transitions.
- Assuming all transitions are valid.
- Incomplete state diagrams.

---

# Key Learnings

- State Transition Testing is a Black Box Testing technique.
- It validates how an application changes from one state to another.
- It is useful for systems with workflows and state-dependent behavior.
- It helps identify invalid state changes.
- It improves software quality by ensuring all transitions are tested.

---

# Interview Questions

### Q1. What is State Transition Testing?

---

### Q2. When should State Transition Testing be used?

---

### Q3. What are the main components of State Transition Testing?

---

### Q4. Give a real-time example of State Transition Testing.

---

### Q5. What is the difference between State Transition Testing and Decision Table Testing?

---

### Q6. What are the advantages of State Transition Testing?

---
