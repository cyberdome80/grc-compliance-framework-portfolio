# Phase 2: Corporate IT Security Policies - Cyberdome GmbH

This document defines the high-level security expectations and operational requirements for all personnel and technical environments at Cyberdome GmbH. To demonstrate compliance in a global workforce, these policies are presented in both English and German.

---

## Policy 1: Identity & Access Management (IAM) Policy

### English Version
1. **Purpose:** To ensure that access to Cyberdome GmbH's networks, cloud environments, and assets is strictly restricted based on the principle of least privilege.
2. **Access Control:** All employees shall be granted access only to the explicit data resources required to perform their daily duties. 
3. **Authentication:** Multi-Factor Authentication (MFA) is strictly mandatory for all corporate accounts, including AWS cloud roots, Active Directory accounts, and email services. Password baselines require a minimum of 14 characters, incorporating upper, lower, numeric, and special symbols.
4. **Account Review:** User access permissions shall be audited quarterly by the security team to identify and revoke stale or orphaned accounts.

### Deutsche Version (Richtlinie zur Identitäts- und Zugriffsverwaltung)
1. **Zweck:** Sicherstellung, dass der Zugriff auf Netzwerke, Cloud-Umgebungen und Vermögenswerte der Cyberdome GmbH streng nach dem Prinzip der minimalen Rechtevergabe (Least Privilege) beschränkt wird.
2. **Zugriffskontrolle:** Allen Mitarbeitern wird nur Zugriff auf die expliziten Datenressourcen gewährt, die zur Erfüllung ihrer täglichen Aufgaben erforderlich sind.
3. **Authentifizierung:** Die Multi-Faktor-Authentifizierung (MFA) ist für alle Unternehmenskonten, einschließlich AWS-Cloud-Roots, Active Directory-Konten und E-Mail-Dienste, zwingend erforderlich. Passwort-Richtlinien erfordern mindestens 14 Zeichen, einschließlich Groß- und Kleinschreibung, Zahlen und Sonderzeichen.
4. **Kontoüberprüfung:** Benutzerzugriffsrechte werden vierteljährlich vom Sicherheitsteam überprüft, um inaktive oder verwaiste Konten zu identifizieren und zu sperren.

---

## Policy 2: Vulnerability Management & Patching Policy

### English Version
1. **Purpose:** To establish a continuous system for identifying, evaluating, and neutralizing technical security flaws within the enterprise infrastructure.
2. **Scanning Frequency:** Automated vulnerability assessments utilizing Nessus must be executed bi-weekly across all external-facing gateways and internal network segments.
3. **Remediation Timelines:** Discovered security flaws must be systematically patched based on their CVSS severity rating:
   * **Critical (CVSS 9.0 - 10.0):** Within 72 hours of discovery.
   * **High (CVSS 7.0 - 8.9):** Within 14 business days.
   * **Medium/Low:** Within 60 business days.
4. **Verification:** Following any critical patch deployment, a follow-up vulnerability scan must be executed to verify the successful closure of the exploit vector.

### Deutsche Version (Richtlinie zum Schwachstellenmanagement und Patchen)
1. **Zweck:** Einrichtung eines kontinuierlichen Systems zur Identifizierung, Bewertung und Neutralisierung technischer Sicherheitsmängel innerhalb der Unternehmensinfrastruktur.
2. **Scan-Häufigkeit:** Automatisierte Schwachstellenbewertungen mit Nessus müssen zweiwöchentlich auf allen externen Gateways und internen Netzwerksegmenten durchgeführt werden.
3. **Behebungsfristen:** Gefundene Sicherheitsmängel müssen systematisch auf Basis ihrer CVSS-Risikobewertung behoben werden:
   * **Kritisch (CVSS 9.0 - 10.0):** Innerhalb von 72 Stunden nach Entdeckung.
   * **Hoch (CVSS 7.0 - 8.9):** Innerhalb von 14 Werktagen.
   * **Medium/Niedrig:** Innerhalb von 60 Werktagen.
4. **Verifizierung:** Nach dem Einspielen kritischer Patches muss ein Folge-Schwachstellenscan durchgeführt werden, um die erfolgreiche Behebung des Angriffsvektors zu bestätigen.

---
*Next Phase: [Phase 3: Cross-Functional Framework Mapping Matrix](./phase3_framework_mapping.md)*


Create Phase 2 Bilingual Corporate Policies
