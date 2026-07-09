# Phase 5: GDPR Data Breach Incident Playbook - Cyberdome GmbH

This playbook details how the GRC team coordinates with technical security analysts (SOC) and legal teams during a suspected data breach involving Personal Identifiable Information (PII), ensuring strict compliance with the EU GDPR 72-hour notification rule.

[Detection & Triage] ---> [Containment & Analysis] ---> [Risk Assessment] ---> [Notification (72 hrs)]
    (SOC / SIEM)              (EDR Isolation)             (GRC Team)               (Legal / Authority)


### Step 1: Detection & Reporting (Hour 0 - 2)
* **Technical Trigger:** **Splunk SIEM** triggers a high-severity alert showing unusual database exfiltration activity via a compromised API Gateway.
* **GRC Action:** Open an incident log in **TheHive**. Verify if the affected database contains European customer data subject to GDPR.

### Step 2: Technical Containment (Hour 2 - 4)
* **Technical Action:** Use **LimaCharlie EDR** to automatically isolate the compromised server from the network to stop data exfiltration. 
* **GRC Action:** Ensure the technical team takes forensic snapshots and keeps exact timestamps of the containment for the final audit trail.

### Step 3: Regulatory Risk Assessment (Hour 4 - 24)
* **GRC Evaluation:** Run a risk assessment to determine if the breach poses a risk to the rights and freedoms of individuals.
  * *Scenario A (No Risk):* Data was fully encrypted with TLS 1.3/AES-256 and the keys are safe. Documentation is filed internally; no external notification is required.
  * *Scenario B (High Risk):* Unencrypted names, emails, or passwords were leaked. Move immediately to Step 4.

### Step 4: Notification Workflow (Hour 24 - 72)
* **Legal Compliance Action:** In accordance with **GDPR Article 33**, draft and submit the official breach notification to the local German Data Protection Authority (*Der Sächsische Datenschutzbeauftragte*) within 72 hours.
* **Customer Communication:** Draft a clear, transparent message to affected users explaining what happened, what data was involved, and what steps they should take (e.g., password resets).


Create Phase 5 GDPR Incident Playbook
