# EN-0008 - Requirements Traceability

Document Number:
EN-0008

Title:
Requirements Traceability

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
STD-REQ-001_Requirements_Standard.md
SYS-001
SYS-002
SYS-003
SYS-004

---

# 1. Purpose

This document establishes the requirements traceability methodology used throughout the ASTRA Autonomous Flight System (AAFS).

The objective of requirements traceability is to ensure that every engineering activity can be traced to an approved requirement and that every requirement can be traced through design, implementation, verification, validation, and mission operations.

---

# 2. Scope

This document applies to all engineering requirements developed as part of the ASTRA program, including:

- Mission Requirements
- System Requirements
- Functional Requirements
- Software Requirements
- Electrical Requirements
- Mechanical Requirements
- Interface Requirements
- Ground System Requirements
- Simulation Requirements
- Verification Requirements
- Safety Requirements

---

# 3. Traceability Philosophy

Traceability ensures that:

- Every requirement has a purpose.
- Every design decision satisfies one or more requirements.
- Every implementation satisfies documented requirements.
- Every requirement has an associated verification method.
- Every verified requirement contributes toward system validation.

No implementation shall exist without a supporting requirement.

No requirement shall exist without an identified engineering purpose.

---

# 4. Requirement Hierarchy

Requirements shall flow from higher-level objectives toward implementation.

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

Lower-level requirements shall reference at least one parent requirement.

---

# 5. Traceability Relationships

Each requirement should maintain traceability to the following where applicable:

Parent Requirement

Child Requirements

Engineering Notebook Entries

Design Documents

Software Modules

Hardware Components

Simulation Models

Test Procedures

Mission Reports

Related Risks

---

# 6. Requirement Traceability Matrix

A traceability matrix shall be maintained throughout the project.

Minimum matrix fields:

| Requirement | Parent | Design | Implementation | Test | Status |
|-------------|--------|--------|----------------|------|--------|
| REQ-SYS-001 | REQ-MIS-001 | SYS-005 | SW-004 | TEST-003 | Draft |

The matrix shall be updated whenever requirements, designs, or verification artifacts change.

---

# 7. Requirement Lifecycle

Requirements shall progress through the following lifecycle:

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

Requirements may only advance after satisfying the criteria of the current stage.

---

# 8. Change Management

Requirement modifications shall:

- Preserve requirement identifiers.
- Record revision history.
- Identify affected engineering documents.
- Identify affected software and hardware.
- Identify affected verification activities.
- Be reviewed before approval.

Requirement identifiers shall never be reused.

Retired requirements shall remain within the project history.

---

# 9. Responsibilities

The project maintainer is responsible for:

- Creating new requirements.
- Approving requirement revisions.
- Maintaining traceability.
- Reviewing requirement consistency.
- Updating affected documentation.

Contributors are responsible for ensuring their work references applicable requirements.

---

# 10. Compliance

Engineering work shall demonstrate compliance with approved requirements before being considered complete.

Compliance shall be demonstrated through one or more of the following:

- Inspection
- Analysis
- Demonstration
- Test

Verification methods shall conform to the ASTRA Requirements Standard.

---

# 11. Future Development

As the ASTRA project matures, automated traceability tools, issue tracking integration, and requirements management software may be introduced.

The principles defined in this document shall remain applicable regardless of implementation tools.

---

# 12. Revision History

| Revision | Date | Description |
|----------|------------|-------------|
| 0.1.0 | 30-06-2026 | Initial document. |

---

# Ad Astra Per Artem