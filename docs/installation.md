\# Installation Guide



\## Lab Environment



| Component | Version |

|----------|---------|

| Ubuntu Server | 22.04 LTS |

| Splunk Enterprise | 9.4.4 |

| Windows | Windows 11 |

| Splunk Universal Forwarder | 9.4.4 |

| Sysmon | Latest |



\---



\## Splunk Server



Install Splunk Enterprise on Ubuntu Server.



Enable boot start.



```bash

sudo /opt/splunk/bin/splunk enable boot-start

```



Start Splunk.



```bash

sudo /opt/splunk/bin/splunk start

```



\---



\## Universal Forwarder



Install the Splunk Universal Forwarder on the Windows endpoint.



Configure `inputs.conf` to monitor:



\- Security

\- System

\- Application

\- Windows PowerShell

\- Microsoft-Windows-Sysmon/Operational



\---



\## Sysmon



Install Sysmon.



```powershell

Sysmon64.exe -accepteula -i sysmonconfig-export.xml

```



\---



\## Verify Data



Run the following search:



```spl

index=wineventlog

```



Events should appear in Splunk.

