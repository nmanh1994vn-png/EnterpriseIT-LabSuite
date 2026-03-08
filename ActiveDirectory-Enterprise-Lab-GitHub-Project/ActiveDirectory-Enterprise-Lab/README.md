# Active Directory Enterprise Lab (Windows Server 2022)

## Overview

This project demonstrates the deployment and configuration of a Windows Server Active Directory environment in a virtualized home lab. The lab simulates a small enterprise infrastructure including a Domain Controller and a domain‑joined Windows client.

Technologies used:
- Windows Server 2022
- Active Directory Domain Services
- Group Policy Management
- File Services
- VMware Workstation
- Windows 10 Client

---

## Lab Architecture

### Host Environment
- Host OS: Windows 11
- Hypervisor: VMware Workstation
- Network Type: NAT

### Domain Controller
- Hostname: DC01
- OS: Windows Server 2022
- Domain: jamesnguyen.local
- IP Address: 192.168.202.133
- DNS Server: 127.0.0.1

### Client Machine
- OS: Windows 10
- Hostname: Client Machine
- Domain Joined: jamesnguyen.local

---

## Active Directory Structure

Organizational Units created to simulate regional departments:

- USA
- Asia
- Europe

Within these OUs:
- User accounts were created
- Security groups were configured
- Users were assigned to appropriate groups

---

## Group Policy Configuration

Group Policy Management Console (GPMC) was installed and used to configure policies including:

- Control Panel restrictions
- Security settings
- Domain policy enforcement

Policies were tested from the domain client machine.

Command used to refresh policies:

gpupdate /force

---

## Domain Join

The Windows 10 client machine was successfully joined to the domain:

jamesnguyen.local

After joining:
- Domain login was verified
- Group policies were applied
- Network connectivity to domain resources was tested

---

## File Services

Shared folders were created on the Windows Server and permissions assigned to domain users.

Network drives were mapped on the domain client and also configured via Group Policy.

---

## Commands Used

ipconfig  
ipconfig /all  
hostname  
gpupdate /force  

---

## Skills Demonstrated

- Active Directory Administration
- Windows Server Management
- Group Policy Configuration
- Domain Networking
- Identity and Access Management
- File Sharing and Permissions
- Virtual Lab Infrastructure

---

## Project Status

This project is currently being expanded with:

- Additional screenshots
- PowerShell automation scripts
- Security policy implementation
- Troubleshooting documentation