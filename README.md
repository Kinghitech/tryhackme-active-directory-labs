# 🧠 TryHackMe – Windows Active Directory Basics Lab

## 📌 Overview
This lab from TryHackMe focuses on foundational **Active Directory (AD)** concepts used in enterprise environments. Active Directory is a centralized identity management system used by most organizations, making it a critical target in cybersecurity.

The lab covers core AD components, user and computer management, authentication, and domain structure.

---

## 🎯 Objectives
- Understand how **Windows Domains** function
- Learn core **Active Directory components**
- Manage **users and groups**
- Manage **computers and Organizational Units (OUs)**
- Understand **Group Policy Objects (GPOs)**
- Learn **authentication methods (Kerberos & NTLM)**
- Understand **Forests, Trees, and Trust relationships**

---

## 🏗️ Lab Environment
- Platform: TryHackMe
- OS: Windows Server (Domain Controller)
- Access Method: RDP
- Tools Used:
  - Active Directory Users & Computers
  - PowerShell
  - Group Policy Management

---

## 🧩 Key Concepts Learned

### 1. Windows Domains
- A **domain** is a centralized network where users and computers are managed.
- Credentials are stored in **Active Directory**.

### 2. Active Directory (AD)
- Centralized database for:
  - Users
  - Groups
  - Computers
- Managed by a **Domain Controller (DC)**

### 3. Users & Groups
- Users = security principals (can authenticate)
- Two group types:
  - Security Groups → permissions
  - Distribution Groups → email lists :contentReference[oaicite:2]{index=2}

### 4. Organizational Units (OUs)
- Used to logically organize:
  - Users
  - Computers
- Enables easier policy application

### 5. Group Policy Objects (GPOs)
- Used to enforce:
  - Security policies
  - Password rules
  - System configurations

### 6. Authentication Methods
- **Kerberos**
  - Ticket-based authentication
- **NTLM**
  - Legacy authentication protocol :contentReference[oaicite:3]{index=3}

### 7. Forests, Trees & Trusts
- **Forest** = highest AD structure
- **Tree** = group of domains
- **Trusts** = allow domains to communicate

---

## 🛠️ Hands-On Tasks Performed

### ✅ Managing Users
- Created and modified user accounts
- Reset user passwords using PowerShell:
```powershell
Set-ADAccountPassword sophie -Reset -NewPassword (Read-Host -AsSecureString -Prompt 'New Password')

### ✅ Managing Computers
Created Organizational Units:
Workstations
Servers
Moved machines into appropriate OUs

### ✅ Delegation
Assigned permissions to allow a user to reset another user’s password

### ✅ Group Policy
Explored how policies are applied across domain users and systems

### 🔐 Security Insights
AD is a high-value target because it controls authentication across the network
Misconfigured permissions can lead to:
Privilege escalation
Lateral movement
Group memberships (e.g., Domain Admins) are critical attack targets

### 🧠 What I Learned
How enterprise environments manage identity and access
The importance of least privilege
How authentication works in real-world networks
Foundational knowledge needed for:
SOC Analyst roles
Active Directory attacks (future labs)

### 🚀 Skills Demonstrated
Active Directory Administration (Basic)
Windows Server Navigation
PowerShell Usage
Identity & Access Management (IAM)
Security Awareness in Enterprise Environments

### 🔗 Lab Link
https://tryhackme.com/room/winadbasics
