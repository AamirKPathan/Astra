# EN-0003 - Repository Standards

Document Number: EN-0003

Title: Repository Standards

Author: Aamir Khan Pathan

Created: 30-06-2026

Last Modified: 30-06-2026

Revision: 0.1.0

Status: Draft

Subsystem: Project Administration

Related Documents: 
EN-0001
EN-0002
EN-0004

---

# 1. Purpose

This document establishes the standards governing the structure, organization, and maintenance of the ASTRA Autonomous Flight System (AAFS) repository. These standards ensure consistency, traceability, maintainability, and scalability throughout the project's lifecycle.

---

# 2. Repository Organization

The ASTRA repository shall be organized by engineering discipline.

Top-level Directories include: 
- Engineering Notebook
- firmware
- ground
- simulation
- hardware
- analysis
- missions
- data
- assets
- docs
- tools
- tests
- .github

Each directory shall contain only files relevant to it's designated purpose.

---

# 3. Directory Standards

Each directory shall contain a README.md file describing its purpose when practical.

Directory names shall remain consisted throughout the project.

New top-level directories shall only be created when a clear engineering need exists.

Duplicate directory structures should be avoided.

---

# 4. File Naming Standards

Engineering notebook documents shall follow the format:
EN-0001_Project_initialization.md

Subsystem documents shall follow the format:
SYS-001_Mission_Requirements.md
SW-001_Software_Architecture.md
MECH-001_Airframe.md
ELEC-001_Power_System.md

For full breakdown of prefixes refer to Astra/Document Templates And Breakdowns/Prefix_Definitions.md

File names shall:

- Use descriptive names.
- Preserve document identifiers.
- Use underscores instead of spaces.
- use the .md extension unless another format is required.

---

# 5. Branch Strategy

Development shall use the following branches:

- main
- develop
- feature/*
- release/*
- hotfix/*

The main branch shall always represent the latest stable revision.

--- 

# 6. Commit Standards

Commits shall represent a single logical change.

Commit messages should follow the format:

docs(EN-0003): update repository standards
feat(nav): implement sensor fusion
fix(control): resolve PID oscillation
hardware(pcb): revise flight computer layout

---

# 7. Documentation Policy

Every significant engineering decision shall be documented.

Implementation should not occur without corresponding engineering documentation.

Engineering documentation is considered part of the implementation

# 8. Repository Maintenance

Unused files shall be removed.

Deprecated files shall be archived rather than deleted.

Large binary files shall be minimized whenever possible.

Repository organization should remain consistent throughout development.

---

# 9. Revision History 
| Revision | Date | Description | 
|----------|------------|-------------| 
| 0.1.0 | 30-06-2026 | Initial document. | 

--- 

# Ad Astra Per Artem