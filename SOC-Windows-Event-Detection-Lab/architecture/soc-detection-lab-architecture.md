# SOC Windows Event Detection Lab Architecture

## Overview

This lab simulates a Security Operations Center (SOC) monitoring environment using Splunk SIEM to detect suspicious activity on a Windows endpoint.

The environment generates attack traffic from an attacker machine and forwards Windows event logs to Splunk for analysis and detection.

---

## Lab Architecture

```
Kali Linux (Attacker)
        │
        ▼
Simulated Attacks
        │
        ▼
Windows 11 Endpoint
        │
        ├── Sysmon
        │      • Process monitoring
        │      • Network activity logging
        │
        └── Windows Event Logs
               • Authentication logs
               • System logs
        │
        ▼
Splunk Universal Forwarder
        │
        ▼
Splunk SIEM
        • Log ingestion
        • Event correlation
        • Security monitoring
```
