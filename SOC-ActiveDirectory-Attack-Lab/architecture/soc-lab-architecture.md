# SOC Active Directory Attack Lab Architecture

## Overview

This lab simulates a real-world Active Directory attack scenario and demonstrates how a Security Operations Center (SOC) can detect suspicious authentication activity.

An attacker machine attempts to perform credential attacks against a Windows domain environment. Security logs are collected and monitored using Splunk SIEM to identify malicious behavior.

---

## Lab Architecture

```
Kali Linux (Attacker)
        │
        ▼
Kerberos / Password Spray Attacks
        │
        ▼
Windows Domain Controller
        │
        ├── Active Directory
        │      • User authentication
        │      • Domain services
        │
        └── Windows Security Logs
               • Authentication events
               • Failed login attempts
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

---

## Components

### Kali Linux
Used as the attacker machine to perform credential attacks such as password spraying.

### Windows Server Domain Controller
Hosts Active Directory Domain Services and manages authentication for the domain.

### Windows Security Logs
Records authentication attempts including successful and failed logins.

### Splunk Universal Forwarder
Collects and forwards Windows event logs to Splunk.

### Splunk SIEM
Central platform used for log analysis, security monitoring, and threat detection.

---

## Attack Simulation Flow

1. Attacker enumerates domain users.
2. Password spraying attack is executed.
3. Windows logs authentication attempts.
4. Logs are forwarded to Splunk.
5. SOC analysts detect suspicious login activity.

---

## Detection Use Case

The lab demonstrates detection of:

- Failed login attempts (Event ID 4625)
- Multiple authentication attempts from a single host
- Suspicious domain login activity
