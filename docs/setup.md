# Lab Setup Guide

This guide outlines how I built my Windows Server 2025 Active Directory home lab in Oracle VirtualBox.

---

## 1. VirtualBox Installation
- Installed Oracle VirtualBox on my Win 11 host machine.
- Configured a dedicated Internal Network to simulate a small enterprise environment without internet exposure.
- Allocated resources:
  - Domain Controller: 2 vCPUs, 4GB RAM, 50GB storage.
  - Clients: 2 vCPU, 4GB RAM, 100GB storage each.

---

## 2. Windows Server 2025 (Domain Controller)
- Created a VM for Windows Server 2025.
- Installed the Active Directory Domain Services (AD DS) role.
- Promoted the server to a Domain Controller and created the domain.
- Configured DNS to support domain resolution.
- Created an internal admin account separate from the built-in Administrator.

---

## 3. Windows 11 Clients
- Deployed four Windows 11 Pro VMs.
- Configured network adapters to connect to the same VirtualBox Internal Network.
- Changed system settings to point DNS to the Domain Controller’s IP.
- Joined each VM to the domain `baltictech.local`.
- One issue I ran into when setting up the first Windows 11 client is that I forgot to enable TPM v2.0 in the settings, which is a baseline requirement for Windows 11.
---

## 4. Active Directory Structure
- Created Organizational Units (OUs) for Admins and Users.
- Added test user accounts (e.g., Helpdesk Admin, Regular Users).
- Grouped accounts based on role for easier management, IT for admins, then HR, Management, and Finance for regular users.

---

## 5. Group Policy Management
- Created and applied Group Policy Objects (GPOs):
- Password length and complexity requirements.
- Account lockout policy.
- Desktop restrictions for regular users.
- Verified application using `gpupdate /force` and Resultant Set of Policy (RSOP).

---

## 6. Testing and Validation
- Logged into Windows 11 clients with domain accounts.
- Verified policy enforcement (password resets, lockouts).
- Tested user permissions vs. helpdesk/admin permissions.
- Practiced account management tasks:
- Unlocking users
- Resetting passwords
- Disabling accounts

---

## Lessons Learned
- How a Domain Controller manages authentication and policies across a network.
- How OUs and GPOs provide structure and security.
- Practical skills in troubleshooting domain joins and DNS issues.
- The difference between admin-level and regular user accounts.
- Windows 11 hardware requirements.

---

