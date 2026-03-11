# SOC Cybersecurity Detection Lab

Hands-on cybersecurity lab demonstrating attack detection using:

- Windows Server / Active Directory
- Windows 11 client
- Sysmon
- Splunk SIEM
- Mimikatz credential dumping

## Lab Goal

Simulate a credential dumping attack and detect it using SIEM logs.

## Lab Components

Domain Controller
- Windows Server 2022
- Active Directory + DNS

Client Machine
- Windows 11 joined to domain

Security Monitoring
- Sysmon for endpoint telemetry
- Splunk for log analysis

## Attack Simulation

Tool used:
- Mimikatz

Commands executed:

```
privilege::debug
sekurlsa::logonpasswords
```

## Detection

Splunk search example:

```
index=main EventCode=3
```

This identifies suspicious network activity and process behavior.

## Skills Demonstrated

- Active Directory administration
- Endpoint telemetry with Sysmon
- SIEM log analysis
- Attack detection workflow
