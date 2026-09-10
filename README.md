# Windows Log Detection — Event IDs & Detection Logic

> Build a small detection engineering lab around Windows Security logs and Sysmon events, then document detection hypotheses and false-positive considerations.

## Objective

This project is a controlled, authorized training lab designed to demonstrate practical Cyber Security skills relevant to a **SOC Analyst / Security Analyst Fresher** role.

## Skills demonstrated

- Security monitoring and investigation
- Windows 10/11, Event Viewer, Sysmon, PowerShell, Wazuh optional, Sigma-style logic
- Evidence-driven documentation
- Basic detection / assessment methodology
- Risk and remediation thinking

## Lab objectives

- Identify useful Windows event sources for SOC monitoring.
- Create detection hypotheses from observable behavior.
- Map evidence to event fields and process context.
- Consider false positives and tuning.
- Document a repeatable investigation path.

## Lab workflow

1. Enable and review Security and Sysmon event channels.
2. Generate benign lab activity such as process creation or repeated failed logons.
3. Identify the event IDs and fields that describe the behavior.
4. Write a detection rule in plain language or Sigma-style YAML.
5. Test the rule logic against the captured event.


## Expected deliverables

- Working lab notes
- Screenshots showing the actual lab state/results
- Findings table
- Remediation notes
- Final lab report

## Evidence policy

**Replace every screenshot placeholder with evidence from your own lab.** Never present generated or edited images as real tool output. Redact usernames, public IP addresses, tokens, API keys and other sensitive data before publishing.

## Screenshots

- `screenshots/01-event-viewer.png`
- `screenshots/02-sysmon-event.png`
- `screenshots/03-detection-rule.png`
- `screenshots/04-test-result.png`
- `screenshots/05-tuning-notes.png`


## Report

See [`lab-report/LAB-REPORT.md`](lab-report/LAB-REPORT.md).

## Safety

Run this project only against systems you own or are explicitly authorized to test. The lab should be isolated from unrelated systems.

## References

- Wazuh documentation: https://documentation.wazuh.com/
- OWASP Juice Shop: https://owasp.org/www-project-juice-shop/
- Nmap documentation: https://nmap.org/book/man.html
- Wireshark User's Guide: https://www.wireshark.org/docs/
- Sysinternals Sysmon: https://learn.microsoft.com/sysinternals/downloads/sysmon
## Repository structure

```text
.
├── README.md
├── lab-report/
│   └── LAB-REPORT.md
├── screenshots/
│   ├── README.md
│   ├── 01-*.png
│   ├── 02-*.png
│   └── ...
├── docs/
│   ├── scope.md
│   ├── findings.md
│   └── remediation.md
├── evidence/
│   └── README.md
└── .gitignore
```
