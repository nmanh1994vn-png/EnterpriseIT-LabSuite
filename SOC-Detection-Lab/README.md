# SOC Detection Lab (Splunk SIEM)

## Overview

This lab simulates a Security Operations Center (SOC) detection workflow.

A Windows 11 virtual machine acts as the monitored endpoint while Kali Linux simulates attacker activity. Sysmon generates detailed telemetry and Splunk collects and analyzes the logs.

This demonstrates real SOC analyst skills such as attack simulation, log analysis, and threat detection.

---

## Lab Environment

Hypervisor: VMware Workstation  
Target Machine: Windows 11 Enterprise  
Attacker Machine: Kali Linux  
SIEM Platform: Splunk Enterprise  
Log Forwarding: Splunk Universal Forwarder  
Endpoint Logging: Sysmon  

---

## Attack Simulation

A TCP SYN scan was performed from Kali Linux using Nmap.

Example command:

nmap -sS <target-ip>

This simulates reconnaissance activity performed by attackers before exploitation.

---

## Detection Queries

### Network Connections (Sysmon)

index=main EventCode=3

This shows network connection activity generated on the Windows endpoint.

### Failed Logins

index=main EventCode=4625

Windows Security Event ID 4625 indicates failed authentication attempts and may indicate brute force activity.

---

## Skills Demonstrated

• SIEM deployment  
• Windows event log analysis  
• Security monitoring  
• Threat detection  
• Network reconnaissance detection
