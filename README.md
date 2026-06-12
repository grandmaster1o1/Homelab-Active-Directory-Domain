# Active Directory Home Lab

## Overview

This project demonstrates the deployment and administration of a Windows Active Directory environment in a virtualized home lab.

The lab simulates a small enterprise network with centralized authentication, DNS services, Group Policy management, and PowerShell automation.

## Technologies Used

- Windows Server 2025
- Windows 11
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Group Policy
- PowerShell
- Hyper-V
- VirtualBox

## Lab Architecture


<img width="1681" height="606" alt="download" src="https://github.com/user-attachments/assets/af82ecaf-aff0-4922-b2e2-8894e1b354d2" />



## Objectives

- Create a Domain Controller VM for Windows Server 2025 - 4GB RAM, 60GB disk
- Install Windows Server and set a static IP (192.168.1.10)
- Install Active Directory and promote to Domain Controller
- Create a second VM with Windows 11 then Point its DNS to the DC IP (192.168.1.10) and join it to the domain
- Create Organizational Units
- Manage users and groups
- Implement Group Policies
- Create shared folders with NTFS + share permissions
- Automate administrative tasks with PowerShell
- Join client machines to the domain

## Environment

| System | Role |
|----------|----------|
| DC01 | Domain Controller |
| WIN11-01 | Client Workstation |
| WIN11-02 | Client Workstation |

## Active Directory Structure

Homelab.local

├── Users

├── Computers

├── IT

├── HR

└── Finance

## Group Policy Configuration

Implemented policies including:

- Password complexity requirements
- Account lockout policy
- Desktop restrictions
- Windows Update settings
- Drive mapping

## PowerShell Automation

Scripts included:

- Bulk user creation
- User disabling
- Group membership management
- OU creation

## Skills Demonstrated

- Active Directory Administration
- Windows Server Management
- DNS and DHCP Configuration
- Group Policy Management
- PowerShell Scripting
- Troubleshooting

## Lessons Learned

- Importance of DNS in Active Directory environments
- Group Policy processing and troubleshooting
- User and permission management best practices
- PowerShell automation for repetitive administrative tasks

## Screenshots

### Domain Controller

[Image]

### Active Directory Users and Computers

[Image]

### Group Policy Management        

[Image]

### Domain Joined Client

[Image]
