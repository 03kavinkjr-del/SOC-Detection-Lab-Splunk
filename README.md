# 🛡️ Enterprise SOC Detection Lab

> A Security Operations Center (SOC) lab built using Splunk Enterprise, Windows Sysmon, and the Splunk Universal Forwarder to collect, analyze, and investigate Windows security events.

---

# 📖 Overview

This project demonstrates the design and implementation of an enterprise-style Security Operations Center (SOC) lab.

The lab centralizes Windows telemetry into Splunk Enterprise, enabling security monitoring, detection engineering, dashboard creation, and incident investigation using real endpoint data.

---

# 🎯 Objectives

- Build a centralized SIEM
- Collect Windows Event Logs
- Deploy Sysmon for endpoint telemetry
- Forward logs using Splunk Universal Forwarder
- Create custom SPL detections
- Build SOC dashboards
- Map detections to MITRE ATT&CK
- Practice threat hunting

---

# 🏗️ Architecture

> Architecture diagram will be added in a future update.

```
Windows 11 Endpoint
        │
        ▼
Splunk Universal Forwarder
        │
     TCP 9997
        │
        ▼
Ubuntu Server 22.04
Splunk Enterprise
        │
        ▼
Search • Dashboards • Alerts
```

---

# 💻 Lab Environment

| Component | Version |
|------------|---------|
| Ubuntu Server | 22.04 LTS |
| Windows | Windows 11 |
| Splunk Enterprise | 9.4.4 |
| Universal Forwarder | 9.4.4 |
| Sysmon | Latest |

---

# 📥 Logs Collected

- Windows Security
- Windows System
- Windows Application
- Windows PowerShell
- Sysmon Operational

---

# 🔍 Detection Engineering

Current detections include:

- Encoded PowerShell
- Brute Force Login
- CMD Execution
- LOLBins
- RDP Logins
- New Service Installation

Each detection includes:

- SPL Query
- MITRE ATT&CK Mapping
- Investigation Guide
- Attack Simulation

---

# 📊 Dashboards

The SOC dashboard includes:

- Security Events
- Sysmon Events
- Failed Logins
- Successful Logins
- PowerShell Activity
- Top Event IDs
- Top Processes

---

# 🛡️ MITRE ATT&CK Coverage

| Detection | ATT&CK |
|------------|---------|
| Encoded PowerShell | T1059.001 |
| Brute Force | T1110 |
| CMD Execution | T1059.003 |
| LOLBins | T1218 |
| RDP | T1021.001 |
| New Service | T1543 |

---

# 📁 Project Structure

```text
SOC-Detection-Lab-Splunk
│
├── architecture/
├── configs/
├── detections/
├── docs/
├── queries/
└── screenshots/
```

---

# 🚀 Future Improvements

- Active Directory Integration
- Wazuh Integration
- Sigma Rules
- Threat Hunting Playbooks
- Automated Incident Response
- Additional MITRE ATT&CK Detections

---

# 👨‍💻 Author

**Kavin Jr**

M.Sc. Cyber Security
