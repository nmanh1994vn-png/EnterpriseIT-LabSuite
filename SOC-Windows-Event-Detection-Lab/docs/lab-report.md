# SOC Windows Event Detection Lab

## Objective

The objective of this lab is to simulate real-world SOC monitoring by generating attack traffic and detecting suspicious activity using Splunk SIEM.

---

## Technologies Used

- Windows 11
- Kali Linux
- Sysmon
- Splunk Enterprise
- Splunk Universal Forwarder

---

## Lab Workflow

1. Install Sysmon on Windows endpoint
2. Install Splunk Enterprise
3. Configure Splunk Universal Forwarder
4. Forward Windows logs to Splunk
5. Simulate attack activity using Kali Linux
6. Analyze logs in Splunk
7. Detect suspicious network and login activity

---

## Detection Scenarios

The following events were detected in Splunk:

- Network scanning activity (Sysmon EventCode 3)
- Failed login attempts (Event ID 4625)

---

## Key Skills Demonstrated

- SIEM log monitoring
- Windows event analysis
- Threat detection
- SOC investigation workflow
