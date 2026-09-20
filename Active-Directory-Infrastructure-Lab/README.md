# Active Directory Infrastructure Lab

## 📌 Overview

Hands-on Active Directory Infrastructure Lab using Windows Server, covering Active Directory Domain Services, Domain Controller deployment, Organizational Units, users, groups, computer management, and Group Policy configuration and validation.

---

## 📑 Table of Contents

- [Project Objectives](#-project-objectives)
- [Technologies & Concepts](#-technologies--concepts)
- [Project Workflow](#-project-workflow)
  - [Windows Server Preparation](#1-windows-server-preparation)
  - [Active Directory Domain Services](#2-active-directory-domain-services)
  - [Domain Controller Deployment](#3-domain-controller-deployment)
  - [Organizational Units](#4-organizational-units)
  - [Users, Groups & Computers](#5-users-groups--computers)
  - [Group Policy](#6-group-policy)
  - [Policy Validation](#7-policy-validation)
- [Configuration & Implementation](#-configuration--implementation)
- [Execution & Validation](#-execution--validation)
- [Skills Demonstrated](#-skills-demonstrated)
- [Documentation](#-documentation)
- [Project Structure](#-project-structure)
- [Project Summary](#-project-summary)

---

## 🎯 Project Objectives

- Deploy a Windows Server Active Directory environment.
- Configure Active Directory Domain Services (AD DS).
- Deploy and configure a Domain Controller.
- Configure DNS for the Active Directory environment.
- Create and organize Organizational Units (OUs).
- Create and manage users and groups.
- Manage computer objects.
- Configure Group Policy Objects (GPOs).
- Apply Group Policy to specific Organizational Units.
- Validate Group Policy application and successful policy updates.

---

## 🛠️ Technologies & Concepts

- Windows Server 2025
- Active Directory Domain Services (AD DS)
- Domain Controller
- Active Directory Users and Computers
- DNS
- Organizational Units (OUs)
- Users & Groups
- Computer Objects
- Group Policy Objects (GPO)
- Group Policy Management
- `gpupdate`

---

# 🔄 Project Workflow

## 1. Windows Server Preparation

Prepared the Windows Server environment for Active Directory deployment.

Activities included:

- Windows Server configuration
- Network configuration
- Server preparation for Active Directory services

---

## 2. Active Directory Domain Services

Installed and configured the Active Directory Domain Services role.

The lab environment used:

```text
Domain: test.local

Activities included:

AD DS role installation
Active Directory configuration
Domain creation
3. Domain Controller Deployment

Configured the Windows Server machine as a Domain Controller.

Activities included:

Domain Controller promotion
Active Directory database configuration
DNS integration
Domain validation
4. Organizational Units

Created and organized Organizational Units to structure the Active Directory environment.

The lab included OUs such as:

FINANCE
HR
SALES

Organizational Units were used to logically organize users, groups, and computer objects and support centralized administration.

5. Users, Groups & Computers

Configured and managed Active Directory objects.

Activities included:

User account creation
Group creation
Computer object management
Organizational Unit assignment
Active Directory object administration
6. Group Policy

Configured Group Policy Objects for centralized management of users and computers.

Activities included:

GPO creation
GPO configuration
GPO linking to Organizational Units
Centralized policy management

The lab included Group Policy configuration for the HR Organizational Unit.

7. Policy Validation

Validated the applied Group Policy configuration using Windows administrative tools and commands.

The lab used:

gpupdate

The policy update was successfully completed and the Computer Policy update was validated.

⚙️ Configuration & Implementation

The Active Directory environment was configured using Windows Server 2025.

Active Directory Configuration
Operating System: Windows Server 2025
Domain: test.local
Role: Domain Controller
Services: AD DS + DNS
Active Directory Structure
test.local
│
├── FINANCE
├── HR
└── SALES

The Organizational Units were used to organize Active Directory objects and apply centralized administrative policies.

Group Policy Configuration

Group Policy was configured and applied to the appropriate Organizational Unit.

Policy application was validated using:

gpupdate
🧪 Execution & Validation

The lab configuration was validated through:

Active Directory Users and Computers
Organizational Unit verification
User and group management
Computer object management
Group Policy configuration
Group Policy application
gpupdate execution
Successful Computer Policy update
🧠 Skills Demonstrated
Active Directory
Active Directory Domain Services
Domain Controller Deployment
Active Directory Users and Computers
User & Group Management
Computer Object Management
Organizational Units
Windows Server
Windows Server 2025
Server Role Configuration
DNS
Active Directory Administration
Group Policy
GPO Creation
GPO Configuration
GPO Linking
Centralized Policy Management
Group Policy Validation
System Administration
Windows Server Administration
Identity & Access Management
Directory Services
Infrastructure Troubleshooting
📸 Documentation

The project documentation contains implementation evidence covering:

Windows Server configuration
Active Directory Domain Services
Domain Controller
DNS
Organizational Units
Users
Groups
Computer Objects
Group Policy
gpupdate
Policy validation
📁 Project Structure
Active-Directory-Infrastructure-Lab/
│
├── README.md
│
└── Active Directory Infrastructure Lab.pdf
⭐ Project Summary

This project demonstrates practical experience in Windows Server and Active Directory administration, including Domain Controller deployment, Active Directory Domain Services, DNS, Organizational Units, user and group management, computer objects, Group Policy configuration, and policy validation.

The lab focuses on building and managing a structured Active Directory environment using Windows Server 2025 and validating centralized administration through Group Policy.


بعد اللصق، اعمل **Commit changes**.

وبعدها نرفع ملف الـPDF الخاص بالـActive Directory داخل نفس الـFolder، بحيث يبقى بالشكل:

```text
Active-Directory-Infrastructure-Lab/
├── README.md
└── Active Directory Infrastructure Lab.pdf
