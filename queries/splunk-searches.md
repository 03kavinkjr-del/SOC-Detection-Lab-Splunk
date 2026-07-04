\# Splunk Searches



\## All Events



```spl

index=wineventlog

```



\---



\## Failed Logins



```spl

index=wineventlog EventCode=4625

```



\---



\## Successful Logins



```spl

index=wineventlog EventCode=4624

```



\---



\## Encoded PowerShell



```spl

index=wineventlog source="WinEventLog:Microsoft-Windows-Sysmon/Operational" EventCode=1

Image="\*powershell.exe"

(CommandLine="\*-enc\*" OR CommandLine="\*-EncodedCommand\*")

```



\---



\## CMD Execution



```spl

index=wineventlog source="WinEventLog:Microsoft-Windows-Sysmon/Operational"

Image="\*cmd.exe"

```



\---



\## LOLBins



```spl

index=wineventlog source="WinEventLog:Microsoft-Windows-Sysmon/Operational"

(Image="\*certutil.exe" OR Image="\*regsvr32.exe" OR Image="\*mshta.exe")

```

