\# Enterprise SOC Detection Lab



\## Overview



This project demonstrates the design and implementation of a Security Operations Center (SOC) detection lab using Splunk Enterprise, Windows Event Logs, Sysmon, and the Splunk Universal Forwarder.



The objective of this lab is to collect endpoint telemetry, centralize logs, build detection rules, create dashboards, and investigate security events using MITRE ATT\&CK–aligned detections.



\---



\## Lab Architecture



Windows 11 Endpoint



\- Sysmon

\- Windows Event Logs

\- Splunk Universal Forwarder



↓



Ubuntu Server 22.04



\- Splunk Enterprise

\- Search \& Reporting

\- Dashboards

\- Alerts

\- Detection Rules



\---



\## Technologies Used



\- Splunk Enterprise 9.4

\- Ubuntu Server 22.04

\- Windows 11

\- Sysmon

\- Splunk Universal Forwarder

\- PowerShell

\- SPL (Search Processing Language)

\- MITRE ATT\&CK Framework



\---



\## Features



\- Windows Event Log Collection

\- Sysmon Event Collection

\- Custom Splunk Searches

\- Security Dashboards

\- Scheduled Alerts

\- Detection Engineering

\- Threat Hunting

\- MITRE ATT\&CK Mapping



\---



\## Current Detections



\- Encoded PowerShell Detection (T1059.001)

\- Brute Force Login Detection (T1110)

\- CMD Execution Detection

\- LOLBins Detection

\- RDP Login Detection

\- New Service Installation Detection



\---



\## Screenshots



Screenshots are available in the `/screenshots` directory.



\---



\## Project Structure



```text

SOC-Detection-Lab-Splunk/

├── architecture/

├── configs/

├── detections/

├── docs/

├── queries/

├── screenshots/

└── README.md

```



\---



\## Future Improvements



\- Active Directory Integration

\- Wazuh Integration

\- Sigma Rule Conversion

\- Additional MITRE ATT\&CK Detections

\- Threat Hunting Playbooks

\- Automated Incident Response



\---



\## Author



Kavin Jr



M.Sc Cyber Security



