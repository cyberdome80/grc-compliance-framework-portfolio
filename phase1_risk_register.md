# Phase 1: ISO 27001 Risk Register & Asset Matrix - Cyberdome GmbH

This document establishes the structured approach used to identify, evaluate, and mitigate risks associated with Cyberdome GmbH's critical information assets. Risks are scored using the formula: **Risk Score = Likelihood (1-5) x Impact (1-5)**.

### Risk Scoring Guide
* **Likelihood:** 1 (Rare) to 5 (Almost Certain)
* **Impact:** 1 (Insignificant) to 5 (Catastrophic)
* **Risk Threshold:** Any score of **12 or higher** requires immediate automated or structural mitigation controls.

| Asset ID | Asset Name / Description | Technical Environment | Threat / Risk Scenario | Initial L | Initial I | Initial Score | Mitigation Control (ISO 27001 / NIST) | Residual Score |
| :--- | :--- | :--- | :--- | :---: | :---: | :---: | :--- | :---: |
| **AST-01** | Production Database (Customer PII) | Cloud (AWS RDS PostgreSQL) | Unauthorized data exfiltration via misconfigured access rights or stolen credentials (GDPR breach). | 4 | 5 | **20 (High)** | Enforce strict Role-Based Access Control (RBAC), mandatory multi-factor authentication (MFA), and TLS 1.3 data encryption at rest. (ISO Annex A.8.12, NIST AC-2) | **5 (Low)** |
| **AST-02** | Corporate User Endpoints | Hybrid (Windows 11 / Active Directory) | Ransomware outbreak spreading via phishing, causing business downtime and data loss. | 4 | 4 | **16 (High)** | Deploy centralized EDR telemetry (LimaCharlie) with automated process isolation scripts and automated Sysmon logging to Splunk SIEM. (ISO Annex A.8.16, NIST SI-4) | **4 (Low)** |
| **AST-03** | Central Logging Environment | Splunk Enterprise On-Premise | Log manipulation or deletion by an internal threat actor to hide unauthorized configuration changes. | 2 | 5 | **10 (Med)** | Restrict log deletion privileges, enforce write-once-read-many (WORM) storage, and set up real-time alerting on configuration changes. (ISO Annex A.8.15, NIST AU-9) | **3 (Low)** |
| **AST-04** | Web Application Gateway | Public Facing API Platform | Exploitation of unpatched software vulnerabilities (e.g., Log4j variants) leading to remote code execution. | 3 | 5 | **15 (High)** | Establish bi-weekly automated Nessus vulnerability scanning schedules paired with immediate patching workflows for critical CVEs. (ISO Annex A.8.8, NIST RA-5) | **6 (Low)** |
| **AST-05** | Internal Network Infrastructure | Local Corporate Network | Lateral movement by an attacker due to an unsegmented network, leading to unauthorized access to internal resources. | 3 | 4 | **12 (High)** | Implement strict network segmentation using pfSense firewalls, deploy Suricata NIDS for real-time traffic monitoring, and block malicious external domains using Pi-hole. (ISO Annex A.8.20, NIST SC-7) | **3 (Low)** |

---
*Next Phase: [Phase 2: Corporate IT Security Policies](./phase2_policies.md)*
