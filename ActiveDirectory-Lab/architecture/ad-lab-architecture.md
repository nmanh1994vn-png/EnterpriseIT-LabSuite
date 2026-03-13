# Active Directory Lab Architecture

## Overview

This lab demonstrates the deployment of an enterprise Windows Active Directory environment using Windows Server 2022 and a domain-joined client machine.

The environment simulates a small corporate network where administrators manage users, computers, and policies through Active Directory and Group Policy.

---

## Lab Architecture

```
Windows 11 Host Machine
        │
        ▼
VMware Workstation
        │
        ├── Domain Controller
        │      Windows Server 2022
        │
        │      Active Directory Domain Services
        │      DNS Server
        │      Group Policy Management
        │
        └── Client Workstation
               Windows 10 / Windows 11
               Domain Joined Endpoint
```

---

## Components

### Domain Controller

Windows Server 2022 configured as the domain controller.

Roles installed:

- Active Directory Domain Services
- DNS Server
- Group Policy Management

---

### Client Workstation

Windows client machine joined to the domain.

Used to test:

- Domain authentication
- Group Policy enforcement
- User management

---

## Key Skills Demonstrated

- Active Directory deployment
- Domain controller configuration
- DNS configuration
- Group Policy management
- Domain joined device management
