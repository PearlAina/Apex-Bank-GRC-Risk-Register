# Apex Bank GRC Enterprise Risk Register & Treatment Framework

An enterprise risk management framework, heat map matrix, and operational risk treatment tracker built for commercial banking environments. This framework aligns with **ISO 27005** and **NIST SP 800-30** standards to evaluate cybersecurity, IT infrastructure, compliance, and physical security threats.

---

## Executive Overview
Apex Bank Ltd. operates critical financial infrastructure subject to strict regulatory oversight (CBN, NDIC, PCI DSS). This repository provides a structured, audit-ready Risk Assessment Framework designed to:
* Quantify inherent and residual risks across enterprise banking domains.
* Apply a standardized **4 × 5 Scoring Matrix** (Likelihood × Impact).
* Track actionable risk treatment plans, due dates, owners, and required audit verification proof.

---

## Assessment Methodology & Heat Map

Risk scores are evaluated on a **1 to 20 scale** using the formula:  
$$\text{Inherent / Residual Risk Score} = \text{Likelihood (1–4)} \times \text{Impact (1–5)}$$

### Risk Bands & Response Criteria
* 🔴 **Priority / High (13 – 20):** Immediate risk treatment required; weekly board and executive oversight.
* 🟡 **Medium (7 – 12):** Mitigation controls scheduled for implementation with active monitoring.
* 🟢 **Low (1 – 6):** Managed via routine operational controls or accepted risk posture.

### Rating Scale Definitions
* **Likelihood (1–4):** `1 - Rare` | `2 - Unlikely` | `3 - Possible` | `4 - Likely`
* **Impact (1–5):** `1 - Negligible` | `2 - Minor` | `3 - Moderate` | `4 - Major` | `5 - Severe`

---

## Summary Risk Register Log

| Risk ID | Risk Description | Category | Inherent Score | Target Mitigation Strategy | Residual Score | Owner | Status |
| :--- | :--- | :--- | :---: | :--- | :---: | :--- | :---: |
| **R2026-01** | Employee Phishing Attack | Cybersecurity | **20** | Enforce mandatory MFA & quarterly phishing simulations | **4** | IT Security Lead | In Progress |
| **R2026-02** | Customer Data Breach | Information Security | **15** | Deploy DLP solution, strict database encryption & access audits | **4** | CISO | Closed |
| **R2026-03** | ATM Network Disruption | Operational | **16** | Procure dual ISP redundant links & UPS at critical ATM sites | **2** | Head of Infrastructure / IT Ops | In Progress |
| **R2026-04** | Unauthorized Privileged Access | Access Management | **20** | Deploy dedicated PAM solution & admin session logging | **2** | IAM Lead | In Progress |
| **R2026-05** | Former Employee Access Active | Access Management | **20** | HR Portal to Active Directory automated API integration | **2** | HR / IAM Lead | In Progress |
| **R2026-06** | Core Banking System Outage | Operational | **16** | Active-Active database clustering & quarterly DR failover tests | **3** | Head of IT Ops | In Progress |
| **R2026-07** | Third-Party SaaS Failure | Third-Party Risk | **16** | Secondary payment fallback providers & continuous monitoring | **6** | Head of Vendor Risk / Procurement | In Progress |
| **R2026-08** | Malware / Ransomware Infection | Cybersecurity | **20** | Deploy EDR, automated patch management & block USB via GPO | **2** | CISO / IT Security Lead | In Progress |
| **R2026-09** | Regulatory Reporting Error | Compliance | **12** | Implement automated RegTech software & validation scripts | **2** | Compliance Officer | Closed |
| **R2026-10** | Physical Access to Server Room | Physical Security | **16** | Dual-factor biometric locks, vendor escorts & 24/7 CCTV | **6** | Head of Physical Security | In Progress |

---

## Actionable Treatment & Audit Verification Plan

| Risk ID | Core Mitigation Action | Due Date | Required Audit Verification / Proof |
| :--- | :--- | :---: | :--- |
| **R2026-01** | Conduct quarterly cybersecurity training & enforce MFA. | 2026-08-31 | Phishing campaign reports & Azure AD MFA enforcement logs. |
| **R2026-02** | Deploy DLP solution and mandate quarterly database access audits. | 2026-08-30 | DLP agent deployment report & database encryption audit sign-off. |
| **R2026-03** | Install dual ISP redundant telecom links and UPS units. | 2026-08-30 | Executed ISP SLA contracts & network failover test logs. |
| **R2026-04** | Deploy PAM solution and automate admin session logging. | 2026-08-30 | CyberArk / PAM vendor Purchase Order & session audit trail. |
| **R2026-05** | Automate real-time HR portal offboarding sync to Active Directory. | 2026-08-30 | API integration specifications & HR-to-AD sync test logs. |
| **R2026-06** | Enforce 1-hour RTO and run quarterly automated DR failover tests. | 2026-09-15 | Disaster Recovery Test Sign-off Sheet & RTO benchmark logs. |
| **R2026-07** | Establish secondary backup vendors & strict SLA downtime penalties. | 2026-09-15 | Vendor SOC 2 Type II reports & fallback routing test results. |
| **R2026-08** | Roll out Endpoint Detection & Response (EDR) and block USB ports. | 2026-09-15 | CrowdStrike/EDR console dashboard & Active Directory GPO exports. |
| **R2026-09** | Deploy RegTech automated reporting software with validation checks. | 2026-09-15 | RegTech software license agreement & test run validation outputs. |
| **R2026-10** | Upgrade server rooms to dual-factor biometrics and expand CCTV. | 2026-09-15 | Vendor site survey report & biometric hardware procurement invoices. |

---

## Repository Deliverables

* **`Apex Bank GRC Risk Register .xlsx`**: Master audit workbook structured into 4 key tabs:
  * **Read me:** Project goals, scope, and ISO 27005 / NIST SP 800-30 framework mapping.
  * **Risk register:** Comprehensive 10-scenario risk log complete with threats, vulnerabilities, controls, and inherent/residual scoring.
  * **Scoring key:** 4x5 Likelihood vs. Impact matrix key and risk band definitions.
  * **Treatment plans:** Mitigation action items, owners, target completion dates, status tracking, and audit proof specifications.
