# Lab Report — Windows Log Detection — Event IDs & Detection Logic

## 1. Executive Summary

**Analyst:** Pham Minh Quang  
**Role target:** Cyber Security Fresher / SOC Analyst  
**Lab status:** Training environment  
**Date:** YYYY-MM-DD  

### Summary

Explain the detection hypothesis, telemetry source, logic, expected signal, likely benign causes and tuning approach.

## 2. Scope

- Lab hosts: `<LAB_HOSTS>`
- Network range / application: `<LAB_SCOPE>`
- Tools: `Windows 10/11, Event Viewer, Sysmon, PowerShell, Wazuh optional, Sigma-style logic`
- Authorization: Self-owned / explicitly authorized training environment

## 3. Objectives

- Identify useful Windows event sources for SOC monitoring.
- Create detection hypotheses from observable behavior.
- Map evidence to event fields and process context.
- Consider false positives and tuning.
- Document a repeatable investigation path.


## 4. Environment

| Component | Value |
|---|---|
| Attacker / analyst VM | `<VALUE>` |
| Target / endpoint | `<VALUE>` |
| Network | `<VALUE>` |
| Tool versions | `<VALUE>` |

## 5. Methodology

1. Enable and review Security and Sysmon event channels.
2. Generate benign lab activity such as process creation or repeated failed logons.
3. Identify the event IDs and fields that describe the behavior.
4. Write a detection rule in plain language or Sigma-style YAML.
5. Test the rule logic against the captured event.


## 6. Evidence

Replace the placeholders below with your own screenshots and filenames.

| ID | Evidence | Observation |
|---|---|---|
| E01 | `../screenshots/01-event-viewer.png` | `<WHAT THE SCREENSHOT PROVES>` |
| E02 | `../screenshots/02-sysmon-event.png` | `<WHAT THE SCREENSHOT PROVES>` |
| E03 | `../screenshots/03-detection-rule.png` | `<WHAT THE SCREENSHOT PROVES>` |
| E04 | `../screenshots/04-test-result.png` | `<WHAT THE SCREENSHOT PROVES>` |
| E05 | `../screenshots/05-tuning-notes.png` | `<WHAT THE SCREENSHOT PROVES>` |


## 7. Findings

| ID | Finding | Severity | Evidence | Recommendation |
|---|---|---|---|---|
| F-01 | `<FINDING>` | Low/Medium/High | E01 | `<REMEDIATION>` |

## 8. Investigation / Analysis

### What happened?
`<Describe the observed behavior in factual terms.>`

### Why does it matter?
`<Describe security relevance and likely impact.>`

### What additional evidence would you collect?
`<Logs, process tree, DNS context, user context, endpoint details, etc.>`

## 9. False Positives / Limitations

`<Describe benign explanations, data gaps and lab limitations.>`

## 10. Remediation / Hardening

- `<ACTION 1>`
- `<ACTION 2>`
- `<ACTION 3>`

## 11. Analyst Takeaways

- `<WHAT I LEARNED>`
- `<WHAT I WOULD AUTOMATE>`
- `<WHAT I WOULD INVESTIGATE NEXT>`

## 12. Conclusion

`<2–4 sentence conclusion focused on evidence, process and next steps.>`
