# Helpdesk Troubleshooting Lab Architecture

## Overview

This lab simulates a typical enterprise IT helpdesk environment where users report issues related to authentication, network connectivity, and printing services.

The environment consists of a Windows Server domain controller and a domain-joined client workstation used to reproduce common IT support tickets.

---

## Lab Architecture

Windows 11 Host Machine
      │
      ▼
VMware Workstation
      │
      ├── Domain Controller
      │   • Windows Server 2022
      │   • Active Directory Domain Services
      │   • DNS Server
      │
      └── Client Workstation
          • Windows 10 / Windows 11
          • Domain Joined Endpoint
