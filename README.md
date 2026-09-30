# Cybersecurity Home Lab

A self-directed, hybrid local/cloud cybersecurity home lab built to practice detection engineering, attack simulation, and blue-team analysis across eight real-world attack and incident scenarios.

## Lab Architecture

- **Attacker VM:** Kali Linux
- **Victim VM:** Ubuntu Server (running DVWA, ModSecurity WAF, Suricata IDS, Wazuh agent)
- **SIEM:** Wazuh (manager, indexer, dashboard) — cloud-hosted on a DigitalOcean VPS
- **Network:** Isolated VirtualBox NAT network, separating the lab from the host machine

The goal throughout: build a realistic attacker/victim/monitoring environment, execute real attack and incident-response scenarios end-to-end, and validate whether the detection stack (WAF → IDS → SIEM) actually catches them — documenting both successes and detection gaps honestly.

*Note: my resume and LinkedIn feature a curated set of 6 highlights for space. This repo contains the full 8-part archive.*

## Lab Reports

| Part | Scenario | Focus |
|---|---|---|
| [Part 1](./part-1-phishing-triage.md) | Phishing Email Triage & SOC Escalation | IOC analysis, threat intel correlation, formal SOC ticket |
| [Part 2](./part-2-phishing-incident-response.md) | Phishing Incident Response | Suricata-to-Wazuh integration, full NIST IR lifecycle |
| [Part 3](./part-3-ssh-brute-force.md) | SSH Brute-Force Detection | SIEM build, MITRE ATT&CK-mapped alerting |
| [Part 4](./part-4-sql-injection.md) | SQL Injection Detection Gap | IDS troubleshooting, root-cause diagnosis |
| [Part 5](./part-5-waf-to-siem.md) | WAF-to-SIEM Log Integration | Log pipeline engineering, live attack validation |
| [Part 6](./part-6-command-injection.md) | Command Injection Testing | WAF evasion testing, SIEM classification gaps |
| [Part 7](./part-7-stored-xss.md) | Stored XSS & Detection Blind Spot | Controlled WAF bypass, single-point-of-failure analysis |
| [Part 8](./part-8-file-upload.md) | File Upload Exploitation | Suricata remediation, exploitability verification |

*(Reports being uploaded — check back if a link isn't live yet.)*

## Skills Demonstrated

Phishing triage & IOC analysis (AbuseIPDB, VirusTotal, URLScan.io) · NIST Incident Response lifecycle · SIEM deployment & administration (Wazuh) · Network IDS (Suricata, Emerging Threats Open) · Web Application Firewall configuration (ModSecurity, OWASP CRS) · MITRE ATT&CK mapping · Compliance framework mapping (NIST 800-53, PCI DSS, GDPR, HIPAA, SOC 2) · Linux system administration · Docker · Cloud VPS administration (DigitalOcean)

## About

Built by Sherman King as part of a career transition from IT support into cybersecurity (SOC Analyst / Identity & Access Management / Threat Hunter). Connect on [LinkedIn](https://www.linkedin.com/in/sherman-king/).
