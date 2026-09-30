# Cybersecurity Home Lab

A self-directed, hybrid local/cloud cybersecurity home lab built to practice detection engineering, attack simulation, and blue-team analysis across real-world attack and incident scenarios.

## Lab Architecture
![Lab Architecture Diagram](./Home%20Lab%201.jpg)
- **Attacker VM:** Kali Linux
- **Victim VM:** Ubuntu Server (running DVWA, ModSecurity WAF, Suricata IDS, Wazuh agent)
- **SIEM:** Wazuh (manager, indexer, dashboard) — cloud-hosted on a DigitalOcean VPS
- **Network:** Isolated VirtualBox NAT network, separating the lab from the host machine

The goal throughout: build a realistic attacker/victim/monitoring environment, execute real attack and incident-response scenarios end-to-end, and validate whether the detection stack (WAF → IDS → SIEM) actually catches them — documenting both successes and detection gaps honestly.

*Note: my resume and LinkedIn feature a curated set of 6 highlights for space. This repo contains the full 8-lab archive.*

## Lab Reports

| Lab | Scenario | Focus |
|---|---|---|
| [Lab 1](./lab-1-phishing-triage.pdf) | Phishing Email Triage & SOC Escalation | IOC analysis, threat intel correlation, formal SOC ticket |
| [Lab 2](./lab-2-phishing-incident-response.pdf) | Phishing Incident Response | Suricata-to-Wazuh integration, full NIST IR lifecycle |
| [Lab 3](./lab-3-ssh-brute-force.pdf) | SSH Brute-Force Detection | SIEM build, MITRE ATT&CK-mapped alerting |
| [Lab 4](./lab-4-sql-injection.pdf) | SQL Injection Detection Gap | IDS troubleshooting, root-cause diagnosis |
| [Lab 5](./lab-5-waf-to-siem.pdf) | WAF-to-SIEM Log Integration | Log pipeline engineering, live attack validation |
| [Lab 6](./lab-6-command-injection.pdf) | Command Injection Testing | WAF evasion testing, SIEM classification gaps |
| [Lab 7](./lab-7-stored-xss.pdf) | Stored XSS & Detection Blind Spot | Controlled WAF bypass, single-point-of-failure analysis |
| [Lab 8](./lab-8-file-upload.pdf) | File Upload Exploitation | Suricata remediation, exploitability verification |

*(Reports being uploaded — check back if a link isn't live yet.)*

## Skills Demonstrated

Phishing triage & IOC analysis (AbuseIPDB, VirusTotal, URLScan.io) · NIST Incident Response lifecycle · SIEM deployment & administration (Wazuh) · Network IDS (Suricata, Emerging Threats Open) · Web Application Firewall configuration (ModSecurity, OWASP CRS) · MITRE ATT&CK mapping · Compliance framework mapping (NIST 800-53, PCI DSS, GDPR, HIPAA, SOC 2) · Linux system administration · Docker · Cloud VPS administration (DigitalOcean)

## About

Built by Sherman King as part of a career transition from IT support into cybersecurity (SOC Analyst / Identity & Access Management / Threat Hunter). Connect on [LinkedIn](https://www.linkedin.com/in/sherman-king/).
