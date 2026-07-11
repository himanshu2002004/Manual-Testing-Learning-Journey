# Day 07 – Severity vs Priority

## What is Severity?

**Severity** refers to the **impact** of a defect on the functionality of the application. It indicates how seriously the defect affects the software's operation.

Severity is usually determined by the **Tester (QA Engineer)** based on the technical impact of the defect.

### Severity Levels

### Critical
A defect that causes the application to crash or blocks a major functionality.

**Example:**
- Application crashes after login.
- Payment transaction fails completely.

---

### High
A major functionality is not working, but the application remains usable.

**Example:**
- User cannot submit a leave request.
- Unable to create a new employee in OrangeHRM.

---

### Medium
A functionality works incorrectly but has an alternative workaround.

**Example:**
- Incorrect validation message displayed.
- Search results are not sorted correctly.

---

### Low
A minor issue that does not affect the application's core functionality.

**Example:**
- UI alignment issue.
- Spelling mistake.
- Incorrect font size.

---

# What is Priority?

**Priority** refers to the **urgency** with which a defect should be fixed. It indicates how quickly the defect needs attention based on business requirements.

Priority is usually decided by the **Project Manager, Product Owner, or Business Analyst**.

### Priority Levels

### High
The defect must be fixed immediately before the next release.

**Example:**
- Login functionality is not working.
- Users cannot complete payment.

---

### Medium
The defect should be fixed in the upcoming release.

**Example:**
- Search functionality is returning incorrect results.

---

### Low
The defect can be fixed in future releases.

**Example:**
- Minor UI issue.
- Cosmetic improvements.

---

# Difference Between Severity and Priority

| Severity | Priority |
|----------|----------|
| Measures the impact of a defect on the application. | Measures how quickly the defect should be fixed. |
| Technical perspective. | Business perspective. |
| Decided by the Tester (QA). | Decided by the Product Owner or Project Manager. |
| Focuses on application functionality. | Focuses on business needs and release timelines. |

---

# Severity vs Priority Matrix

| Severity | Priority | Example |
|----------|----------|---------|
| High | High | Login button is not working. |
| High | Low | Admin report generation fails, but the feature is rarely used. |
| Low | High | Company logo is incorrect on the homepage before product launch. |
| Low | Low | Minor spelling mistake in the footer. |

---

# Real-Time Examples

## High Severity – High Priority

**Scenario:** User cannot log in using valid credentials.

**Impact:** Core functionality is blocked.

**Fix:** Immediate.

---

## High Severity – Low Priority

**Scenario:** Report generation fails for a feature used only by administrators once a year.

**Impact:** Major functionality affected.

**Business Urgency:** Low.

---

## Low Severity – High Priority

**Scenario:** Incorrect company logo displayed on the homepage before a product launch.

**Impact:** Small technical issue.

**Business Urgency:** High because it affects branding.

---

## Low Severity – Low Priority

**Scenario:** Typographical error in the "Contact Us" page.

**Impact:** Very small.

**Business Urgency:** Can be fixed later.

---

# Can Severity and Priority be Different?

**Yes.**

Severity and Priority are independent of each other.

For example:

- A spelling mistake on the homepage may have **Low Severity** but **High Priority** if it affects the company's reputation.
- A rarely used report feature may have **High Severity** but **Low Priority** because it does not affect most users.

---

# How to Decide Severity?

Ask yourself:

- Does the application crash?
- Is the core functionality blocked?
- Is there any workaround?
- How many users are affected?

---

# How to Decide Priority?

Ask yourself:

- Does this affect the customer?
- Will this delay the release?
- Is it a business-critical feature?
- Does management want it fixed immediately?

---

# Best Practices

- Assign severity based on the technical impact of the defect.
- Assign priority based on business importance.
- Do not confuse severity with priority.
- Discuss uncertain cases with the development and product teams.
- Always provide proper justification while assigning severity and priority.

---

# Common Mistakes

- Assuming High Severity always means High Priority.
- Assigning Priority based only on technical impact.
- Ignoring business requirements while deciding Priority.
- Using incorrect severity levels without proper analysis.

---

# Key Learnings

- Severity measures the impact of a defect on the application.
- Priority measures the urgency of fixing the defect.
- Severity is decided by the Tester.
- Priority is decided by the Product Owner or Project Manager.
- A defect can have any combination of Severity and Priority depending on its technical impact and business importance.

---

# Interview Questions

### Q1. What is Severity?

---

### Q2. What is Priority?

---

### Q3. Who decides Severity and Priority?

---

### Q4. Can a defect have High Severity and Low Priority?

---

### Q5. Can a defect have Low Severity and High Priority?

---

### Q6. Which is more important, Severity or Priority?

---

# Summary

- **Severity = Impact of the defect**
- **Priority = Urgency to fix the defect**
- **Severity is technical.**
- **Priority is business-oriented.**
- **A defect can have different combinations of Severity and Priority depending on the situation.**
