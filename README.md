<h1>Securing Payment Systems: PCI DSS 4.0 Compliance Assessment</h1>

<h2>Description</h2>

As a compliance consultant, I conducted a PCI DSS 4.0 assessment for a retail company's payment processing environment. The objective was to evaluate alignment with PCI DSS standards, identify critical compliance gaps, and provide a prioritized remediation roadmap to strengthen cardholder data protection.

<h2>Key Findings</h2>

- **Unencrypted Cardholder Data:** PANs stored in plain text within daily backups, creating high breach exposure.

- **Weak Access Controls:** Shared admin credentials, no MFA on internal portals.

- **Outdated Protocols:** TLS 1.0/1.1 still enabled in parts of the environment.

- **Lack of Secure SDLC:** No formal code reviews or security testing practices in development.

 - **Limited Monitoring:** Logs collected but no centralized review or alerting.

- **No Incident Response (IR) Plan:** Absence of a documented or tested IR process.

<h2>Remediation Plan </h2>

- **Encryption:** Apply AES-256 encryption for stored PANs; update backup strategy.

- **Access Control:** Enforce unique logins, role-based access, and MFA across admin systems.

- **TLS Hardening:** Disable TLS 1.0/1.1, enforce TLS 1.2+.

- **Secure SDLC:** Introduce code reviews, OWASP Top 10 training, and SAST/DAST integration.

- **Monitoring:** Deploy centralized SIEM with real-time alerting.

- **Incident Response:** Develop, test, and document IR procedures with assigned roles.

<h2>Results & Business Impact</h2>

- Clear remediation roadmap for PCI DSS alignment within 60 days.

- Eliminated major risks around data storage, access, and monitoring.

- Delivered leadership briefing tying compliance actions to customer trust, financial risk reduction, and long-term business resilience

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
