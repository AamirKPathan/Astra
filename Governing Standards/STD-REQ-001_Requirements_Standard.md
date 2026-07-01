# ASTRA Requirements Standard

Document Number:
STD-REQ-001

Title:
Requirements Standard

Author:
Pathan

Created:
30-06-2026

Last Modified:
30-06-2026

Revision:
0.1.0

Status:
Draft

Subsystem:
Project Administration

Related Documents:
EN-0004
EN-0008

---

# 1. Purpose

This document establishes the standard for writing, organizing, identifying, verifying, and maintaining requirements throughout the ASTRA Autonomous Flight System (AAFS).

All engineering requirements shall conform to this standard.

---

# 2. Requirement Philosophy

Requirements define **what** the system shall accomplish.

Requirements shall **not** specify implementation details unless explicitly required.

Implementation decisions belong within design documentation.

---

# 3. Characteristics of a Good Requirement

A requirement shall be:

- Clear
- Concise
- Unambiguous
- Measurable
- Verifiable
- Achievable
- Traceable
- Necessary
- Consistent
- Atomic (one requirement per statement)

---

# 4. Requirement Language

Requirements shall use mandatory language.

Approved wording:

- shall
- shall not

Avoid:

- should
- could
- may
- might
- preferably

Example:

✓ The system shall record telemetry at a minimum rate of 100 Hz.

✗ The system should record telemetry quickly.

---

# 5. Requirement Format

Each requirement shall contain:

Requirement ID

Requirement Title

Description

Rationale

Verification Method

Priority

Status

Parent Requirement

Related Documents

---

Example

Requirement ID:
REQ-SYS-001

Title:
Telemetry Logging

Description:
The flight computer shall record telemetry at a minimum rate of 100 Hz.

Rationale:
Provides sufficient temporal resolution for post-flight analysis.

Verification:
Test

Priority:
High

Status:
Draft

Parent Requirement:
REQ-MIS-001

---

# 6. Requirement Categories

Mission Requirements

REQ-MIS-###

System Requirements

REQ-SYS-###

Functional Requirements

REQ-FNC-###

Software Requirements

REQ-SW-###

Electrical Requirements

REQ-ELEC-###

Mechanical Requirements

REQ-MECH-###

Interface Requirements

REQ-INT-###

Verification Requirements

REQ-TEST-###

Operational Requirements

REQ-OPS-###

Safety Requirements

REQ-SAFE-###

Recovery Requirements

REQ-REC-###

Ground System Requirements

REQ-GCS-###

Simulation Requirements

REQ-SIM-###

---

# 7. Requirement Hierarchy

Mission Requirements

↓

System Requirements

↓

Subsystem Requirements

↓

Component Requirements

↓

Implementation

↓

Verification

↓

Validation

Every lower-level requirement shall trace to at least one higher-level requirement.

---

# 8. Requirement Priority

Critical

High

Medium

Low

---

# 9. Requirement Status

Draft

Proposed

Approved

Implemented

Verified

Validated

Deprecated

Retired

---

# 10. Verification Methods

I — Inspection

A — Analysis

T — Test

D — Demonstration

Every requirement shall define at least one verification method.

---

# 11. Requirement Traceability

Every requirement shall maintain traceability to:

Higher-level requirement

Engineering notebook entry

Design document

Implementation

Test

Mission (if applicable)

No requirement shall exist without traceability.

---

# 12. Requirement Numbering

Requirement numbers shall never be reused.

Deleted requirements shall remain reserved.

Example:

REQ-SYS-001

REQ-SYS-002

REQ-SYS-003

If REQ-SYS-002 is removed:

REQ-SYS-001

REQ-SYS-002 (Retired)

REQ-SYS-003

---

# 13. Requirement Lifecycle

Draft

↓

Review

↓

Approved

↓

Implemented

↓

Verified

↓

Validated

↓

Retired

---

# 14. Requirement Traceability Matrix

| Requirement | Parent | Design | Implementation | Test | Status |
|-------------|--------|--------|----------------|------|--------|
| REQ-SYS-001 | REQ-MIS-001 | SYS-005 | SW-010 | TEST-004 | Approved |

---

# 15. Requirement Example

Requirement ID:
REQ-SYS-014

Title:
Attitude Estimation

Description:
The flight computer shall estimate vehicle attitude at a minimum update frequency of 100 Hz.

Rationale:
Provides sufficient bandwidth for closed-loop flight control.

Verification:
T

Priority:
Critical

Status:
Approved

Parent Requirement:
REQ-MIS-002

---

# 16. Revision History

| Revision | Date | Description |
|----------|------------|-------------|
| 0.1.0 | 30-06-2026 | Initial document. |

---

# Ad Astra Per Artem