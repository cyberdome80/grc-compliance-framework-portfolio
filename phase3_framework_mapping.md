# Phase 3: Cross-Functional Framework Mapping Matrix - Cyberdome GmbH

This matrix maps Cyberdome GmbH's technical security capabilities and tools against standard global compliance frameworks. It proves that a single technical control simultaneously satisfies requirements across multiple regulatory standards.

| Technical Control / Action | Primary Security Tool | ISO/IEC 27001:2022 Control | NIST SP 800-53 Rev 5 | SOC 2 Type II Criteria | GDPR Legal Requirement |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Enforcing centralized end-to-end event and security telemetry logging. | **Splunk Enterprise SIEM** | **A.8.15** (Logging) | **AU-2** (Audit Events) | **CC7.2** (Monitoring & Security Vulnerabilities) | **Article 32** (Security of Processing - Traceability) |
| Automated monitoring of endpoint processes and real-time malicious activity containment. | **LimaCharlie EDR** | **A.8.16** (Monitoring activities) | **SI-4** (Information System Monitoring) | **CC7.3** (Cyber Threat Detection & Mitigation) | **Article 32** (Technical Measures for Ongoing Availability) |
| Bi-weekly automated vulnerability scanning and asset posture validation. | **Nessus Professional** | **A.8.8** (Management of technical vulnerabilities) | **RA-5** (Vulnerability Monitoring and Scanning) | **CC7.1** (Vulnerability Management Operations) | **Article 32** (Regular Testing and Evaluation of Effectiveness) |
| Hardening endpoint access boundaries via centralized directory structures and identity management. | **Active Directory / Group Policy (GPO)** | **A.5.15** (Access control) / **A.8.2** (Privileged access rights) | **AC-2** (Account Management) / **IA-2** (Identification and Authentication) | **CC6.1** (Access Amendment & Authorization Controls) | **Article 25** (Data Protection by Design and by Default) |
| Isolating critical network subnets and tracking structural border traffic deviations. | **pfSense Firewall / Suricata NIDS** | **A.8.20** (Network security) / **A.8.21** (Security of network services) | **SC-7** (Boundary Protection) | **CC6.6** (Perimeter Defense & Logical Boundary Protections) | **Article 32** (Confidentiality and Integrity of Networks) |

---
*Next Phase: [Phase 4: Internal Audit Evidence Checklist](./phase4_audit_readiness.md)*


Create Phase 3 Cross-Functional Framework Mapping Matrix
