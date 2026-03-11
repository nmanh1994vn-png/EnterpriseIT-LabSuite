# SOC Lab Report

## Environment

Host OS: Windows 11  
Hypervisor: VMware Workstation  

VMs:
- DC01 – Windows Server 2022
- WIN11 – Domain joined workstation

## Security Tooling

Sysmon installed for system telemetry.

Splunk used as SIEM platform.

## Attack Simulation

Mimikatz executed on the Windows client to dump credentials.

## Detection

Splunk queries used:

index=main EventCode=3

Logs showed suspicious activity triggered by attack execution.
