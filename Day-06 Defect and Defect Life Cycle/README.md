# Day 06 – Defect and Defect Life Cycle

## What is a Defect?

A Defect is a flaw or issue in a software application where the actual behavior differs from the expected behavior specified in the requirements. Defects are identified during testing and reported to the development team for resolution.

**Example:**
If a user enters valid login credentials but is unable to access the dashboard, it is considered a defect.

---

# Terminologies

### Error
A mistake made by a developer while writing the code.

### Defect (Bug)
A flaw identified during the testing phase due to an error in the application.

### Failure
When the software fails to perform its expected functionality because of one or more defects.

---

# Causes of Defects

- Misunderstood requirements
- Incorrect coding
- Design flaws
- Environment issues
- Integration problems
- Configuration issues
- Database errors
- Poor exception handling

---

# Defect Attributes

A defect report generally contains the following information:

- Defect ID
- Defect Summary
- Module
- Description
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Environment
- Build Version
- Status
- Assigned To
- Reporter
- Attachment/Screenshot
- Comments

---

# Defect Severity

Severity indicates the impact of the defect on the application's functionality.

### Critical
Application crashes or major functionality is unavailable.

**Example:** Application crashes after clicking the Login button.

### High
Major functionality is affected.

**Example:** User cannot transfer money.

### Medium
Functionality works but with incorrect behavior.

**Example:** Incorrect validation message is displayed.

### Low
Minor issues with little impact.

**Example:** Typographical or UI alignment issues.

---

# Defect Priority

Priority indicates how quickly a defect should be fixed.

### High
Must be fixed immediately.

### Medium
Should be fixed in the upcoming release.

### Low
Can be fixed in future releases.

---

# Severity vs Priority

| Severity | Priority |
|----------|----------|
| Indicates the impact of the defect | Indicates the urgency to fix the defect |
| Decided by Tester | Decided by Product Owner/Manager |
| Technical impact | Business impact |

---

# Defect Life Cycle

A defect goes through multiple stages from identification until closure.

```text
  New
   ↓
Assigned
   ↓
  Open
   ↓
 Fixed
   ↓
 Retest
   ↓
Verified
   ↓
 Closed
```

Possible alternate states:

```text
Rejected
Duplicate
Deferred
Not a Bug
Cannot Reproduce
Reopened
```

---

# Defect Status Explained

### New
Tester reports the defect.

### Assigned
The defect is assigned to a developer.

### Open
Developer starts working on the defect.

### Fixed
Developer fixes the issue and updates the status.

### Retest
Tester retests the fixed functionality.

### Verified
Tester confirms that the defect has been resolved.

### Closed
The defect is closed successfully.

### Reopened
The defect still exists after fixing.

### Rejected
Developer rejects the defect because it is invalid.

### Duplicate
The defect has already been reported.

### Deferred
The defect fix is postponed to a future release.

### Cannot Reproduce
Developer is unable to reproduce the issue.

### Not a Bug
The reported behavior is expected according to the requirements.

---

# Defect Life Cycle Flow

```text
Defect Found
      ↓
New
      ↓
Assigned
      ↓
Open
      ↓
Fixed
      ↓
Retest
      ↓
Verified
      ↓
Closed
```

Alternative Flow

```text
New
 ↓
Assigned
 ↓
Open
 ├── Fixed → Retest → Verified → Closed
 ├── Rejected
 ├── Duplicate
 ├── Deferred
 ├── Cannot Reproduce
 └── Not a Bug
```

---

# Components of a Good Defect Report

A good defect report should include:

- Clear Summary
- Detailed Description
- Accurate Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Supporting Evidence (Screenshots/Videos)
- Environment Details

---

# Example Defect Report

**Defect ID:** BUG_001

**Module:** Login

**Summary:** User can access the Dashboard after logout using the browser Back button.

**Steps to Reproduce**

1. Login with valid credentials.
2. Logout.
3. Click the browser Back button.

**Expected Result**

The user should be redirected to the Login page.

**Actual Result**

The Dashboard is displayed.

**Severity**

High

**Priority**

High

**Status**

New

---

# Best Practices for Defect Reporting

- Write a clear summary.
- Mention exact steps to reproduce.
- Attach screenshots or videos.
- Mention the environment and browser details.
- Avoid duplicate defects.
- Verify the issue before reporting.
- Assign the correct severity and priority.

---

# Common Defect Types

- Functional Defects
- UI Defects
- Validation Defects
- Performance Defects
- Security Defects
- Compatibility Defects
- Database Defects
- Integration Defects
- Usability Defects

---

# Key Learnings

- A defect is any deviation from the expected behavior.
- Every defect follows a defined life cycle before closure.
- Severity and Priority are different concepts.
- A well-written defect report helps developers reproduce and fix issues faster.
- Proper defect management improves software quality and ensures successful releases.

---

# Interview Questions

### Q1. What is a Defect?

---

### Q2. What is the difference between Error, Defect, and Failure?

---

### Q3. What is Defect Life Cycle?

---

### Q4. What is the difference between Severity and Priority?
---

### Q5. What are the common defect statuses?

---

### Q6. What makes a good defect report?
