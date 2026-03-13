# Helpdesk Troubleshooting Lab Report

## Overview

This lab simulates common IT helpdesk support tickets encountered in enterprise environments. The objective is to demonstrate structured troubleshooting methods used by IT support technicians to diagnose and resolve user issues efficiently.

The scenarios focus on three typical helpdesk incidents:

- Domain login issue
- Network connectivity problem
- Printer service issue

---

# Lab Environment

Host System
- Windows 11 Host Machine
- VMware Workstation

Virtual Machines
- Windows Server 2022 Domain Controller
- Windows Client Workstation (Domain Joined)

Administrative Tools
- Active Directory Users and Computers
- Command Prompt
- Windows Services
- Printer Management
- Network Diagnostic Commands

---

# Ticket 1 — User Cannot Login to Domain

## Problem

A user reports that they cannot log in to their workstation. The system indicates that the account is locked after multiple failed login attempts.

## Investigation

Steps performed:

1. Open **Active Directory Users and Computers**
2. Locate the affected domain user
3. Review account properties
4. Check account lockout status
5. Verify password policy

## Root Cause

The user account was locked due to repeated incorrect password attempts.

## Resolution

1. Unlock the user account in Active Directory
2. Reset the user password
3. Verify the user can successfully log in to the domain

---

# Ticket 2 — User Cannot Access Network

## Problem

The user reports they cannot access network resources or the internet from their workstation.

## Investigation

Troubleshooting commands used:
ipconfig
ping


Steps performed:

1. Run **ipconfig** to verify IP address assignment
2. Confirm subnet mask and default gateway
3. Test connectivity using **ping**
4. Verify DNS resolution

## Resolution

Network connectivity was restored after confirming:

- Correct IP configuration
- Working default gateway
- Successful ping response
- Proper DNS resolution

---

# Ticket 3 — Printer Not Working

## Problem

User reports that documents cannot be printed and appear stuck in the printer queue.

## Investigation

Troubleshooting steps:

1. Check installed printers
2. Verify printer queue status
3. Inspect **Print Spooler Service**
4. Restart the print spooler service

## Resolution

1. Restart the **Print Spooler Service**
2. Clear the printer queue
3. Verify printer connectivity

Printing functionality was successfully restored.

---

# Skills Demonstrated

This lab demonstrates key IT support skills:

- Helpdesk troubleshooting methodology
- Active Directory user account management
- Windows network diagnostics
- DNS troubleshooting
- Printer service troubleshooting
- Windows system administration

---

# Key Takeaways

This lab demonstrates common helpdesk troubleshooting procedures used in enterprise IT environments. It highlights systematic diagnosis, problem isolation, and resolution using standard administrative tools.

