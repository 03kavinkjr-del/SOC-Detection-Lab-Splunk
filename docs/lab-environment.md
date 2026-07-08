\# Lab Environment



\## SOC Server



| Item | Value |

|------|-------|

| Operating System | Ubuntu Server 22.04 LTS |

| SIEM | Splunk Enterprise 9.4.4 |



\---



\## Endpoint



| Item | Value |

|------|-------|

| Operating System | Windows 11 |

| Agent | Splunk Universal Forwarder |

| Monitoring | Sysmon |



\---



\## Logs Collected



\- Security

\- System

\- Application

\- Windows PowerShell

\- Microsoft-Windows-Sysmon/Operational



\---



\## Network



Windows Endpoint



↓



Splunk Universal Forwarder



↓



TCP 9997



↓



Splunk Enterprise



↓



Search / Dashboards / Alerts

