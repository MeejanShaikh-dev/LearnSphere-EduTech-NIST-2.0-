# LearnSphere EdTech — NIST CSF 2.0 Cybersecurity Gap Assessment

## Project Overview

A hands-on **Cybersecurity GRC portfolio project** assessing a simulated EdTech organization, **LearnSphere EdTech**, against selected outcomes from the **NIST Cybersecurity Framework (CSF) 2.0**.

The project evaluates the organization's existing cybersecurity posture, establishes a realistic target state, calculates maturity gaps, prioritizes remediation activities, and develops a practical **12-month cybersecurity remediation roadmap**.

The assessment places particular emphasis on the protection of **student and children's data**, including access governance, privacy requirements, data inventory, retention, monitoring, incident response, and recovery.

---

## Organization Context

**Organization:** LearnSphere EdTech
**Industry:** Education Technology
**Environment:** Cloud-hosted Learning Management System
**Primary Cloud:** AWS
**Project Type:** Cybersecurity GRC / NIST CSF 2.0 Gap Assessment

### Assessment Scope

The assessment covers:

* AWS production infrastructure
* LMS applications
* Production databases
* Identity & Access Management
* Source-code repositories
* CI/CD environment
* Backup and recovery
* Security monitoring / SIEM
* Employee endpoints
* Relevant personnel and process owners
* Relevant third-party service providers

### Primary Risk Focus

* Children's data
* Student personal information
* Student-record access
* Parental-consent governance
* Data minimization
* Data retention and disposal
* Privacy and contractual requirements

---

## Project Objectives

The assessment was designed to:

1. Define the cybersecurity assessment boundary.
2. Assess the existing cybersecurity posture.
3. Establish realistic target maturity.
4. Quantify maturity gaps.
5. Prioritize the most material deficiencies.
6. Develop a practical remediation roadmap.
7. Define management KPIs for continuous monitoring.
8. Produce management-ready GRC reporting.

---

## NIST CSF 2.0 Coverage

The assessment covers all six NIST CSF 2.0 Functions:

| Function | Code | Current | Target |  Gap | Priority    |
| -------- | ---- | ------: | -----: | ---: | ----------- |
| Govern   | GV   |    1.75 |   3.00 | 1.25 | High        |
| Identify | ID   |    1.75 |   3.00 | 1.25 | High        |
| Protect  | PR   |    1.75 |   3.25 | 1.50 | Critical    |
| Detect   | DE   |    1.75 |   3.00 | 1.25 | High        |
| Respond  | RS   |    2.00 |   3.00 | 1.00 | Medium-High |
| Recover  | RC   |    1.75 |   3.00 | 1.25 | Medium      |

**Total selected outcomes assessed:** 24

---

## Executive Results

| Metric                   |                  Result |
| ------------------------ | ----------------------: |
| Overall Current Maturity |         **1.79 / 4.00** |
| Overall Target Maturity  |         **3.04 / 4.00** |
| Overall Maturity Gap     |                **1.25** |
| Functions Assessed       |                   **6** |
| Outcomes Assessed        |                  **24** |
| Largest Function Gap     |      **Protect — 1.50** |
| Highest-Priority Outcome | **PR.AA-05 — Critical** |
| Remediation Horizon      |           **12 Months** |

The **Protect** Function has the largest function-level gap at **1.50** and is classified as Critical because of the significance of student-record access and authorization governance.

---

## Assessment Methodology

The project uses an internal **0–4 evidence-based maturity scale**:

| Score | Rating              | Definition                                                       |
| ----: | ------------------- | ---------------------------------------------------------------- |
|     0 | Not Performed       | No credible evidence of implementation                           |
|     1 | Ad Hoc              | Informal, inconsistent or reactive practice                      |
|     2 | Repeatable          | Some consistency, but documentation or measurement is incomplete |
|     3 | Defined             | Documented, assigned and consistently implemented                |
|     4 | Managed / Optimized | Measured, reviewed and continuously improved                     |

### Important Methodology Note

The **0–4 maturity scale is an internal project methodology**.

It is kept separate from **NIST CSF 2.0 Tier categorization**.

The assessment primarily targets **Tier 3 — Repeatable** across the six Functions, with Respond starting at Tier 2 because some risk-informed response capability already exists.

---

## Current vs Target State

The target maturity was generally established using:

**Target = Current + 1**

An exception was intentionally applied to **PR.AA-05**, where the target was set to **Level 4** because student-record access governance requires stronger measurement, review and continuous improvement.

### PR.AA-05 — Student-Record Access Governance

**Current:** 2
**Target:** 4
**Gap:** 2
**Priority:** Critical

Key improvement areas include:

* Role-Based Access Control
* Least privilege
* Separation of duties
* Privileged-access governance
* Quarterly access certification
* Joiner-Mover-Leaver integration
* Exception tracking
* Access governance metrics

---

## Major Gap Themes

The assessment identified several cross-functional cybersecurity improvement areas:

### 1. Children's-Data Governance

Translate legal, privacy, contractual and parental-consent requirements into operational cybersecurity and data-processing requirements.

### 2. Student-Data Inventory

Establish an authoritative inventory of sensitive and designated student data, including ownership, purpose, location, sensitivity, flows and retention.

### 3. Student-Record Access Governance

Strengthen RBAC, least privilege, privileged access, separation of duties and recurring access certification.

### 4. Data Lifecycle Management

Improve data minimization, retention schedules, secure disposal and disposal verification.

### 5. Security Monitoring

Improve correlation between IAM, application and student-record access events.

### 6. Incident Response

Formalize severity classification, evidence handling, communication and response playbooks for student-data incidents.

### 7. Recovery & Continual Improvement

Convert incident and exercise lessons learned into owned, tracked and verified improvement actions.

---

## Top 6 Priority Gaps

| Rank | Gap    | NIST Outcome | Function | Current → Target | Priority | Score |
| ---: | ------ | ------------ | -------- | ---------------- | -------- | ----: |
|    1 | GAP-09 | PR.AA-05     | Protect  | 2 → 4            | Critical |  4.70 |
|    2 | GAP-01 | GV.OC-03     | Govern   | 1 → 3            | High     |  4.70 |
|    3 | GAP-06 | ID.AM-07     | Identify | 1 → 3            | High     |  4.70 |
|    4 | GAP-12 | PR.DS-10     | Protect  | 1 → 3            | High     |  4.50 |
|    5 | GAP-16 | DE.AE-04     | Detect   | 1 → 3            | High     |  4.05 |
|    6 | GAP-24 | RC.IM-01     | Recover  | 1 → 3            | Medium   |  3.25 |

---

## Remediation Prioritization Model

The project uses an internal weighted prioritization model.

| Factor                            | Weight |
| --------------------------------- | -----: |
| Regulatory / Contractual Exposure |    30% |
| Risk-Reduction Impact             |    35% |
| Cost / Effort                     |    15% |
| Dependency / Enablement           |    20% |

### Weighted Score

**Priority Score =**

`Regulatory / Contractual × 30%`
`+ Risk Reduction × 35%`
`+ Cost / Effort × 15%`
`+ Dependency / Enablement × 20%`

This is an **internal project prioritization methodology**, not an official NIST CSF scoring mechanism.

---

## 12-Month Remediation Roadmap

### 0–3 Months — Foundations

Focus on immediate risk reduction and control foundations.

* Student-record access governance
* RBAC and least privilege
* Children's-data requirements
* Parental-consent governance
* Student-data inventory foundation
* Retention and disposal baseline
* Detection correlation design

### 3–6 Months — Operationalize & Measure

Convert foundations into repeatable operating processes.

* Access certification and metrics
* Privacy-by-design workflow
* Complete student-data inventory
* Deletion enforcement
* Monitoring effectiveness metrics
* MTTD / MTTI tracking
* Improvement-action tracking

### 6–12 Months — Validate & Reassess

Measure effectiveness and close residual gaps.

* Control-effectiveness testing
* Recovery and resilience exercises
* Ransomware / database compromise scenarios
* Third-party security assurance
* RTO/RPO validation
* NIST CSF target-profile reassessment
* Residual-risk review
* Next remediation cycle

---

## Management KPIs

The project defines measurable indicators to monitor progress and effectiveness.

| KPI                                 | Target / Direction                                       | Cadence   |
| ----------------------------------- | -------------------------------------------------------- | --------- |
| Student-record access certification | 100% reviewed quarterly                                  | Quarterly |
| Privileged-access exceptions        | Zero unauthorized standing privileged access             | Monthly   |
| Student-data inventory coverage     | 100% designated data stores and major flows mapped       | Monthly   |
| Retention / disposal verification   | Evidence available for scheduled deletion and exceptions | Quarterly |
| Security monitoring coverage        | Critical IAM/application/data telemetry covered          | Monthly   |
| Incident detection metrics          | MTTD / MTTI trend monitoring                             | Monthly   |
| Improvement action closure          | Owner, due date, evidence and effectiveness verification | Monthly   |

---

## Project Deliverable Chain

```text
Assessment Scope
       ↓
Maturity Rating Methodology
       ↓
Current Maturity Assessment
       ↓
Target Maturity Assessment
       ↓
Gap Calculation
       ↓
Gap Prioritization
       ↓
12-Month Remediation Roadmap
       ↓
Management KPIs
       ↓
Final Assessment & Recommendation
       ↓
NIST CSF Reassessment
```

---

## Project 1 Traceability

This project builds upon **Project 1: LearnSphere EdTech ISO/IEC 27001:2022 ISMS**.

| Project 1                  | Project 2                      |
| -------------------------- | ------------------------------ |
| Organizational Context     | NIST CSF Govern                |
| Asset Register             | NIST CSF Identify              |
| Risk Register              | Gap Prioritization             |
| Statement of Applicability | Existing Security Context      |
| Internal Audit             | Evidence / Control Validation  |
| Corrective Actions         | Remediation Roadmap            |
| Management Review          | Management KPIs & Reassessment |

Together, the projects demonstrate how **ISO/IEC 27001:2022 and NIST CSF 2.0 can support complementary GRC activities** across governance, risk, controls, assessment and continual improvement.

---

## Evidence Planning

The assessment identifies evidence categories required to validate the target state.

### Governance Evidence

* Security policies
* Privacy requirements
* Risk assessments
* Management-review records
* Governance decisions

### Data Evidence

* Data inventory
* Data-flow diagrams
* Consent records
* Retention schedules
* Disposal evidence

### IAM Evidence

* IAM exports
* RBAC matrix
* MFA reports
* Access-certification records
* Privileged-account register

### Cloud & Security Evidence

* AWS configuration reports
* Security findings
* SIEM log-source inventory
* Detection rules
* Security dashboards

### Incident & Recovery Evidence

* Incident register
* Response playbooks
* Exercise reports
* Backup reports
* Recovery-test results
* RTO/RPO evidence

### Third-Party Evidence

* Supplier assessments
* Security questionnaires
* Contracts
* Assurance reports
* Monitoring records

---

## Repository Structure

```text
LearnSphere-NIST-CSF-2.0-Gap-Assessment/
│
├── README.md
│
├── 01_Project_Context/
│   ├── Project_Scope
│   └── Organization_Context
│
├── 02_Current_Profile/
│   └── Current_Maturity_Assessment
│
├── 03_Target_Profile/
│   └── Target_Maturity_Assessment
│
├── 04_Gap_Assessment/
│   └── Gap_Calculation
│
├── 05_Gap_Prioritization/
│   └── Priority_Analysis
│
├── 06_Remediation_Roadmap/
│   └── 12_Month_Roadmap
│
├── 07_KPI_KRI/
│   └── Management_Metrics
│
├── 08_Evidence_Plan/
│   └── Evidence_Requirements
│
├── 09_Executive_Report/
│   └── Master_Assessment_Report
│
└── 10_Visuals/
    ├── LinkedIn_Graphics
    └── Project_Diagrams
```

---

## Key Skills Demonstrated

### Cybersecurity GRC

* NIST CSF 2.0
* Cybersecurity Governance
* Risk Assessment
* Gap Assessment
* Risk-Based Prioritization
* Remediation Planning
* Control Effectiveness
* Management Reporting

### Information Security

* IAM Governance
* RBAC
* Least Privilege
* Data Protection
* Data Lifecycle Management
* Security Monitoring
* Incident Response
* Recovery & Resilience

### Compliance & Privacy

* Children's-data governance
* Parental-consent requirements
* Data minimization
* Retention and disposal
* Regulatory / contractual considerations
* Evidence-based compliance

### GRC Documentation

* Current / Target Profiles
* Gap Register
* Prioritization Matrix
* Remediation Roadmap
* KPI Framework
* Evidence Plan
* Executive Reporting

---

## Standards & References

* **NIST Cybersecurity Framework (CSF) 2.0**
* **NIST CSF 2.0 Organizational Profiles**
* **NIST SP 1301 — Developing Organizational Profiles**
* **NIST SP 1302 — Cybersecurity Framework 2.0 Tiers**
* **ISO/IEC 27001:2022** — contextual reference from Project 1
* **India DPDP Act** — regulatory context for the simulated EdTech environment

---

## Key Takeaway

This project demonstrates that a cybersecurity gap assessment is not simply a checklist exercise.

The GRC process connects:

**Business Context → Data → Assets → Current State → Target State → Gaps → Risk → Prioritization → Remediation → Evidence → Measurement → Reassessment**

The objective is not simply to close the maximum number of gaps.

The objective is to reduce the most material exposure, establish sustainable controls, measure their effectiveness, and continuously improve the organization's cybersecurity posture.

---

## Disclaimer

This is a **simulated cybersecurity GRC portfolio project** created for educational, professional development and portfolio demonstration purposes.

LearnSphere EdTech is a fictional organization. The maturity ratings, prioritization scores, assessment assumptions and remediation roadmap are project-specific methodologies and should not be interpreted as an official NIST assessment, certification, audit opinion or representation of a real organization's security posture.

---

## Author

**Meejan Shaikh**
GRC Analyst | Information Security | Risk & Compliance | Cybersecurity Governance

**Project:** LearnSphere EdTech — NIST CSF 2.0 Cybersecurity Gap Assessment

**Portfolio Focus:** GRC | NIST CSF 2.0 | ISO 27001 | Risk Management | Compliance | Information Security

---

## Related Project

**Project 1 — LearnSphere EdTech ISO/IEC 27001:2022 ISMS**

The NIST CSF 2.0 assessment was developed as a continuation of the LearnSphere EdTech ISMS/GRC portfolio work.

---

**LearnSphere EdTech**
*Learning Today. A Safer Tomorrow.*
