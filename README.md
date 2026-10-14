# Security Operations | Incident Response | Detection Engineering

I work on monitoring, incident response, and detection engineering, mostly on Windows endpoints and Microsoft cloud.

GIAC GCIH | GIAC GSEC | CompTIA Security+

## Projects

### [Triage Engine](https://github.com/oasunsec/triage-engine)

Takes Windows EVTX files or live collection and turns them into findings, incidents, timelines, and an HTML case report.

* Built-in behavioral detections plus optional Sigma rules
* Sysmon and Windows Security event analysis, mapped to MITRE ATT&CK
* Alerts grouped into findings and incidents, with tuning overrides
* Review queue with owners, notes, and dispositions

### [Honey Token Detection](https://github.com/oasunsec/honey-token-detection)

Decoy Word and HTML files that call home when opened. The receiver runs on Azure Container Apps and sends events to Microsoft Sentinel.

* FastAPI receiver deployed with Bicep
* Separate Sentinel rules for first hits, scanner-like requests, and repeats
* KQL hunting queries
* Redacted evidence from opening the decoy in Word to the Sentinel incident
* Cost notes and teardown steps

### [Azure Data Exfiltration Defense Lab](https://github.com/oasunsec/azure-data-exfiltration-defense-lab)

A synthetic financial file in Azure Blob Storage and SharePoint, and the controls meant to keep it from leaving, each tested with a real request.

* Storage auth and IP firewall, scoped RBAC and Azure Policy, deployed with Bicep
* Conditional Access MFA and a Sentinel detection for denied writes
* Purview DLP with a custom classifier that blocked an external guest
* KQL investigation, redacted evidence and a full teardown record

### [Cybersecurity Portfolio](https://github.com/oasunsec/cybersecurity-portfolio)

Four lab write-ups with the raw artifacts kept:

* PCAP investigation where I decoded the exfiltrated data and recovered a stolen API key
* Vulnerability scan where I separated real findings from scanner noise and fixed them behind a reverse proxy
* SQL injection login bypass with saved requests and a retest
* RDP detection rule and the reasoning behind keeping it

### [ShareSafe](https://github.com/oasunsec/share-safe)

A single-page browser tool that finds and redacts secrets, email addresses, and personal file paths before you paste logs into a ticket or public issue. Nothing leaves the browser. [Try it](https://oasunsec.github.io/share-safe/).

## Currently working on

* Microsoft Sentinel and KQL
* Azure and Microsoft Entra ID security
* Defender for Cloud
* Incident response playbooks
* Detection tuning and automation
* Threat intelligence enrichment

## Tools

**SIEM & Detection:** Microsoft Sentinel, Splunk, Elastic, KQL, Sigma, Sysmon

**Cloud & Identity:** Azure, Entra ID, Defender for Cloud, RBAC, Conditional Access

**Security Operations:** Incident response, threat hunting, detection engineering, MITRE ATT&CK

**Automation:** Python, PowerShell, REST APIs

**Network:** Wireshark, Zeek, Snort
