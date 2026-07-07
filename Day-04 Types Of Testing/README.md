# Day 4 - Types of Software Testing

---

# What are Types of Testing?

Types of Testing are different approaches used to verify various aspects of a software application. Each type of testing has a specific objective and helps identify different kinds of defects.

---

# Types of Software Testing

# Classification of Software Testing

```text
Software Testing
│
├── White Box Testing
│   ├── Unit Testing
│   ├── Statement Coverage
│   ├── Branch Coverage
│   ├── Path Coverage
│   ├── Loop Testing
│   └── Condition Coverage
│
├── Black Box Testing
│   │
│   ├── Functional Testing
│   │   ├── Integration Testing
│   │   ├── System Testing
│   │   ├── User Acceptance Testing (UAT)
│   │   ├── Smoke Testing
│   │   ├── Sanity Testing
│   │   ├── Regression Testing
│   │   └── Retesting
│   │
│   ├── Non-Functional Testing
│   │   ├── Performance Testing
│   │   ├── Load Testing
│   │   ├── Stress Testing
│   │   ├── Volume Testing
│   │   ├── Scalability Testing
│   │   ├── Security Testing
│   │   ├── Compatibility Testing
│   │   ├── Usability Testing
│   │   ├── Reliability Testing
│   │   └── Recovery Testing
│   │
│   ├── Ad Hoc Testing
│   └── Exploratory Testing
│
└── Gray Box Testing

```

# White Box Testing

---

## What is White Box Testing?

White Box Testing is a testing technique where the tester has complete access to the source code and verifies the internal working of the application.

---

## Other Names of White Box Testing

- Glass Box Testing
- Clear Box Testing
- Transparent Box Testing
- Structural Testing
- Code-Based Testing
- Open Box Testing

---

## Objectives of White Box Testing

- Verify the internal code and logic.
- Ensure every statement and branch executes correctly.
- Identify coding errors.
- Detect security vulnerabilities.
- Improve code quality.
- Remove dead or unused code.

---

## Who Performs White Box Testing?

- Developers
- Software Engineers
- Automation Test Engineers (sometimes)

---

## Types of White Box Testing

### 1. Statement Coverage

### 2. Branch Coverage

### 3. Path Coverage

### 4. Loop Testing

### 5. Condition Coverage

---

## Advantages

- Finds coding errors early.
- Improves code quality.
- Optimizes application performance.
- Identifies dead code.
- Increases code coverage.
- Helps improve application security.

---

## Disadvantages

- Requires programming knowledge.
- Time-consuming for large applications.
- Cannot identify missing business requirements.
- Expensive if the application is large.

---

## Real-Time Example

Consider the following Login code:

```java
if(username.equals("admin") && password.equals("admin123"))
{
    System.out.println("Login Successful");
}
else
{
    System.out.println("Invalid Credentials");
}
```

A developer performing White Box Testing checks:

- Whether both conditions execute correctly.
- Whether the `if` block executes.
- Whether the `else` block executes.
- Whether all possible code paths are covered.

The focus is on testing the **internal code**, not just the output.

---

# Black Box Testing

---

## What is Black Box Testing?


Black Box Testing is a testing technique where the tester validates the functionality of an application without knowing its internal implementation.

---

## Other Names of Black Box Testing

- Functional Testing
- Specification-Based Testing
- Behavioral Testing
- Closed Box Testing

---

## Objectives of Black Box Testing

- Verify business requirements.
- Validate application functionality.
- Ensure the application behaves correctly.
- Identify functional defects.
- Improve user experience.

---

## Who Performs Black Box Testing?

- Manual Test Engineers
- QA Engineers
- Test Analysts
- End Users (during User Acceptance Testing)

---

## Types of Black Box Testing

- Functional Testing
- Non Functional Testing
- Adhoc Testing
- Exploratory Testing

---

## Types of Functional Testing

- Integration Testing
- System Testing
- User Acceptance Testing (UAT)
- Smoke Testing
- Sanity Testing
- Regression Testing
- Retesting

---

## Types of Non-Functional Testing

- Performance Testing
- Load Testing
- Stress Testing
- Volume Testing
- Scalability Testing
- Security Testing
- Compatibility Testing
- Usability Testing
- Reliability Testing
- Recovery Testing

---

## Advantages

- No programming knowledge required.
- Tests the application from the user's perspective.
- Helps validate business requirements.
- Easy to perform.
- Suitable for Manual Testing.

---

## Disadvantages

- Internal code is not tested.
- Limited code coverage.
- Difficult to identify the exact cause of defects.
- Some execution paths may remain untested.

---

## Real-Time Example

Application: E-Commerce Website

Login Page

The tester performs the following checks:

- Enter valid username and password.
- Verify successful login.
- Enter an incorrect password.
- Verify an error message is displayed.
- Leave fields empty.
- Verify validation messages appear.
- Click the Login button and ensure the application responds correctly.

The tester does **not** know how the login code is written or how the database validates the credentials.

The focus is only on whether the functionality works correctly.

---

## Key Learnings

- Black Box Testing validates application functionality.
- Internal source code is not required.
- Manual Test Engineers mainly perform Black Box Testing.
- It verifies software from the end user's perspective.

---

# Difference Between White Box Testing and Black Box Testing

| White Box Testing | Black Box Testing |
|-------------------|-------------------|
| Internal code is visible. | Internal code is hidden. |
| Focuses on code and logic. | Focuses on functionality. |
| Programming knowledge is required. | Programming knowledge is not required. |
| Performed mainly by Developers. | Performed mainly by Test Engineers. |
| Tests statements, branches, loops, and paths. | Tests application features and business requirements. |
| Also called Structural Testing. | Also called Functional Testing or Behavioral Testing. |
| Finds coding defects. | Finds functional defects. |

---

# Interview Questions

### Q1. What is White Box Testing?

---

### Q2. What is Black Box Testing?

---

### Q3. Who performs White Box Testing?

---

### Q4. Who performs Black Box Testing?

---

### Q5. Which testing technique is mostly used in Manual Testing?

---

### Q6. Which testing technique requires programming knowledge?

---

### Q7. Give a real-time example of Black Box Testing.

---

### Q8. Give a real-time example of White Box Testing.

---

### Easy Way to Remember

**White Box Testing = Know the Code → Test the Logic**

**Black Box Testing = Don't Know the Code → Test the Functionality**
