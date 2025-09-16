<h1>PCI DSS Compliance Assessment for a Retail Company's Payment System</h1>

<h2>Description</h2>

I conducted a PCI DSS 4.0 assessment for a retail company's payment processing environment. The objective was to evaluate alignment with PCI DSS standards, identify critical compliance gaps, and provide a prioritized remediation roadmap to strengthen cardholder data protection.

<h2>Key Findings</h2>

The assessment revealed several high-risk gaps. Cardholder data was stored unencrypted, with PANs found in plain text within daily backups, which significantly increased breach exposure. 

Access controls were weak, as administrators relied on shared credentials and internal portals lacked multi-factor authentication. Outdated security protocols were also in use, with TLS 1.0 and 1.1 still enabled in parts of the environment.

The development function had no secure SDLC practices in place, meaning code reviews and security testing were absent. Monitoring was limited to log collection without centralized review or alerting, and the organization had neither a documented incident response plan nor evidence of testing IR procedures.


<h2>Remediation Plan </h2>

To address these issues, I developed a remediation plan that included encrypting stored PANs with AES-256 and updating the backup strategy, enforcing unique logins with role-based access controls and MFA, and disabling obsolete TLS versions in favor of TLS 1.2 and above. 

I also recommended embedding security into the SDLC through structured code reviews, OWASP Top 10 developer training, and SAST/DAST integration. For monitoring, I proposed deploying a centralized SIEM with real-time alerting, while for incident response I designed and documented a process with defined roles, responsibilities, and testing requirements.

<h2>Business Impact</h2>

The outcome of this engagement was a clear remediation roadmap to achieve PCI DSS alignment within 60 days. The company eliminated major risks tied to data storage, access control, and monitoring. I also provided leadership with a strategic briefing that linked compliance improvements directly to enhanced customer trust, reduced financial risk, and stronger long-term business resilience.









<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
