# Phase 4: Internal Audit Evidence Checklist - Cyberdome GmbH

This checklist shows exactly what proof we give to an auditor to prove that Cyberdome GmbH follows its security rules. It bridges our daily technical work with the compliance checkboxes.

### 1. Topic: Identity & Access Management (ISO 27001 A.5.15 / A.8.2)
* **What the auditor asks to see:** Proof that only authorized people have access to critical systems and that Multi-Factor Authentication (MFA) is actually active.
* **The technical proof we provide:** 
  * A exported user list from AWS and Active Directory showing that all active accounts have the MFA flag turned "On".
  * A screenshot of the Group Policy Object (GPO) configuration showing that passwords must be at least 14 characters long.

### 2. Topic: Threat Monitoring & Incident Management (ISO 27001 A.8.15 / A.8.16)
* **What the auditor asks to see:** Proof that we are actively looking for network threats and keeping system logs safely.
* **The technical proof we provide:**
  * A live walk-through of our Splunk SIEM dashboard showing active incoming logs from our endpoints and firewalls.
  * A copy of our recent automated rule configurations from LimaCharlie EDR showing how the system automatically isolates a compromised machine.

### 3. Topic: Vulnerability Management (ISO 27001 A.8.8)
* **What the auditor asks to see:** Proof that we scan our network for security flaws and fix them on time.
* **The technical proof we provide:**
  * A PDF report exported directly from Nessus showing the results of our last bi-weekly vulnerability scan.
  * Patch logs showing that critical vulnerabilities were successfully updated and closed within our 72-hour policy window.

### 4. Topic: Network Security (ISO 27001 A.8.20)
* **What the auditor asks to see:** Proof that our internal network is segmented and protected from unauthorized entry.
* **The technical proof we provide:**
  * A diagram of our network architecture showing how our internal subnets are separated.
  * A copy of our firewall rules from pfSense showing that all unneeded external ports are blocked.


Create Phase 4 Internal Audit Evidence Checklist
