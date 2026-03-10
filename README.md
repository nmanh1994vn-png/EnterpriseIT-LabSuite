
# Enterprise IT Lab Suite

## Overview

This repository contains a collection of hands-on enterprise IT labs designed to simulate real-world IT infrastructure and support scenarios.

The lab environment includes multiple virtual machines consisting of a Windows Server 2022 Domain Controller and Windows client systems configured in a simulated enterprise network.

The labs demonstrate practical skills in:

- Windows Server administration
- Microsoft 365 cloud management
- Active Directory identity management
- IT helpdesk troubleshooting

---

## Labs Included


## Active Directory Enterprise Lab
Deployment and configuration of a Windows Server 2022 Active Directory environment.

Key Tasks:
- Installed Windows Server 2022 and configured a Domain Controller
- Created Organizational Units (OUs), users, and security groups
- Implemented Group Policy settings
- Joined Windows client machines to the domain

Lab Files:
[Active Directory Lab](ActiveDirectory-Lab)

---

## Microsoft 365 / Entra ID / Intune Lab
Configuration of a Microsoft 365 tenant and cloud identity management environment.

Key Tasks:
- Created Microsoft 365 tenant
- Configured users and security groups in Entra ID
- Assigned licenses and enabled MFA
- Configured and explored device management capabilities in Microsoft Intune
  
Lab Files:
[Microsoft 365 / Entra ID / Intune Lab](Microsoft365-EntraID-Intune-Lab)

---

## Helpdesk Troubleshooting Lab
Simulation of common IT support troubleshooting scenarios in a Windows environment.

Key Tasks:
- Investigated user login issues using Active Directory
- Diagnosed network connectivity problems using ipconfig and ping
- Resolved printer issues by restarting Print Spooler service
- Practiced standard helpdesk troubleshooting workflow

Lab Files:
[Helpdesk Troubleshooting Lab](Helpdesk-Troubleshooting-Lab)

### SOC Detection Lab
→ Splunk SIEM deployment  
→ Sysmon endpoint logging  
→ Attack simulation using Kali Linux  
→ Threat detection using Splunk queries  

[Open SOC Detection Lab](./SOC-Detection-Lab)
---

# Technologies Used

- Windows Server 2022
- Windows 11
- Active Directory
- Microsoft 365
- Microsoft Entra ID
- Microsoft Intune
- VirtualBox
- Networking tools (ping, ipconfig, nslookup)

---

# Purpose of This Repository

This project demonstrates practical enterprise IT skills through hands-on lab environments, focusing on:

- Identity and access management
- Cloud administration
- Windows infrastructure
- IT support troubleshooting
