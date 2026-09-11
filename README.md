# windows-active-directory-home-lab
Windows Server and Active Directory home lab demonstrating practical IT support, domain administration and troubleshooting skills.

# Windows Active Directory Home Lab

## Overview

I built a virtual Windows enterprise environment to develop practical IT support and Service Desk skills.

Using Oracle VirtualBox, I deployed Windows Server 2022 and Windows 11 Pro virtual machines, configured Active Directory Domain Services (AD DS), created a domain controller, managed domain users and groups, and joined a Windows 11 client to the domain.

The lab provides a safe environment for practising user administration, permissions, networking and troubleshooting scenarios commonly encountered in IT support environments.

## Lab Environment

### Platforms
- Oracle VirtualBox
- Windows Server 2022
- Windows 11 Pro

### Directory & Network Services
- Active Directory Domain Services (AD DS)
- Domain Name System (DNS)

### Networking
- TCP/IP

## Virtual Lab Setup

I created two virtual machines in Oracle VirtualBox to simulate a small Windows enterprise environment:

- **Windows Server 2022** — provides the server infrastructure for the Active Directory domain.
- **Windows 11 Pro** — represents an end-user workstation that can be joined to and managed within the domain.

The virtualised environment allows me to practise Windows administration, identity management and troubleshooting without affecting my physical host system.

![Oracle VirtualBox environment showing Windows 11 Pro and Windows Server 2022 virtual machines](screenshots/01-virtualbox-environment.png)


## Active Directory Domain Setup

I installed Active Directory Domain Services (AD DS) on Windows Server 2022 and promoted the server to a Domain Controller for the `LAB.local` domain.

Using Active Directory Users and Computers, I created organisational units for accounts and groups and created domain user accounts for centralised identity management.

![Active Directory Users and Computers showing the LAB.local domain and user accounts](screenshots/02-active-directory-users.png)

## Domain-Joined Windows 11 Client

I configured the Windows 11 Pro client to use the Domain Controller for DNS and joined the workstation to the `LAB.local` domain.

I then successfully signed into the workstation using a domain user account created in Active Directory, verifying domain connectivity and authentication.

![Windows 11 domain account and domain membership verification](screenshots/03-domain-client-verification.png)

## Skills Demonstrated

- Built and configured Windows 11 Pro and Windows Server 2022 virtual machines
- Installed and configured Active Directory Domain Services (AD DS)
- Promoted Windows Server 2022 to a Domain Controller
- Created and administered Active Directory users, groups and organisational units
- Configured DNS for Active Directory client connectivity
- Joined a Windows 11 Pro workstation to an Active Directory domain
- Managed user account provisioning, password resets and disabled accounts
- Configured group-based NTFS permissions for departmental resources
- Created and mapped shared network folders on a domain-joined workstation

## Service Desk Support Scenarios

I completed practical support scenarios within the lab to develop experience with common Windows and Active Directory administration tasks.

### Ticket 001 — Disabled Domain Account
Investigated a domain login issue, identified a disabled Active Directory account and restored user access.

[View Ticket 001](tickets/001-disabled-domain-account.md)

### Ticket 002 — Forgotten Password
Reset a domain user's password, required a password change at next logon and verified successful authentication.

[View Ticket 002](tickets/002-password-reset.md)

### Ticket 003 — New Starter Account
Created a new Active Directory domain account for an authorised new starter and verified domain authentication.

[View Ticket 003](tickets/003-new-starter-account.md)

### Ticket 004 — Finance Shared Folder Access
Assigned a user to a departmental security group, configured group-based folder permissions and mapped the network share.

[View Ticket 004](tickets/004-finance-folder-access.md)
