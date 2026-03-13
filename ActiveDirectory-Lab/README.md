# Active Directory Enterprise Lab

## Overview

This lab demonstrates the deployment and configuration of a Windows Server Active Directory environment in a virtualized enterprise network.

The environment simulates a small corporate infrastructure where a Windows Server Domain Controller manages domain users, authentication, and network services.

The goal of this lab is to practice common system administration tasks used by IT support and system administrators.

---

## Lab Architecture

```
Windows 11 Host Machine
│
└── VMware Workstation
    │
    ├── Domain Controller
    │   ├── Windows Server 2022
    │   ├── Active Directory Domain Services
    │   └── DNS Server
    │
    └── Client Machine
        ├── Windows 10 / Windows 11
        └── Domain Joined Endpoint
```

---

## Technologies Used

- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS
- Windows Client
- VMware Workstation

---

## Key Tasks Performed

- Installed Windows Server 2022
- Promoted server to Domain Controller
- Installed Active Directory Domain Services
- Configured DNS
- Created domain users and groups
- Joined Windows client to the domain
- Verified domain authentication

---

## Skills Demonstrated

- Active Directory administration
- Domain management
- User and group management
- DNS configuration
- Windows enterprise infrastructure

---

## Screenshots

Screenshots demonstrating the configuration process are available in the **screenshots** folder.
