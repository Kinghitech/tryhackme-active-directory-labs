# 🔐 Active Directory Security Testing Basics Lab (TryHackMe)

This repository documents my hands-on completion of the **Active Directory Security Testing Basics** module from TryHackMe.

The purpose of this project is to demonstrate practical experience with **Active Directory enumeration, authentication, credential security, privilege escalation, and lateral movement** in a simulated enterprise environment.

---

## 🎯 Objectives

* Understand the fundamentals of Windows Active Directory
* Understand how Active Directory authentication works
* Identify common Active Directory attack vectors
* Perform basic Active Directory enumeration
* Perform authenticated enumeration
* Understand how credentials are stored and exposed
* Explore Active Directory lateral movement techniques
* Identify common AD security weaknesses and their mitigations

---

# 🧪 Labs Completed

## 1. Active Directory Basics

### Topics Covered

* Active Directory fundamentals
* Domain Controllers
* Users and Groups
* Organizational Units (OUs)
* Group Policy
* Domain structure

### Hands-On Actions

* Explored Active Directory domain structure
* Identified users, groups, and computers
* Examined the role of Domain Controllers
* Reviewed Organizational Units
* Explored Group Policy concepts

### Key Takeaways

* Active Directory provides centralized identity and access management
* Domain Controllers authenticate users and manage directory services
* Groups are commonly used to manage permissions at scale
* Misconfigured permissions can create security risks

---

## 2. Intro to AD Authentication

### Topics Covered

* Active Directory authentication
* Kerberos
* NTLM
* Authentication tickets
* Domain authentication

### Hands-On Actions

* Examined how users authenticate within an AD environment
* Explored Kerberos authentication
* Reviewed NTLM authentication
* Identified differences between modern and legacy authentication protocols

### Key Takeaways

* Kerberos is the primary authentication protocol used by modern Active Directory environments
* NTLM is an older authentication mechanism
* Authentication weaknesses can be leveraged to compromise accounts
* Proper authentication controls are critical to enterprise security

---

## 3. Intro to AD Breaching

### Topics Covered

* Username enumeration
* Password spraying
* Credential attacks
* Coercion
* Account security
* Mitigations

### Hands-On Actions

* Performed username enumeration
* Explored password spraying techniques
* Examined how weak authentication controls can expose accounts
* Investigated coercion concepts
* Reviewed defensive mitigations

### Security Takeaways

* Weak passwords increase the risk of password spraying
* Username enumeration can provide attackers with valid account names
* MFA can significantly reduce the impact of stolen credentials
* Account lockout and monitoring policies can help detect attacks

---

## 4. AD: Basic Enumeration

### Topics Covered

* Network enumeration
* Domain discovery
* User enumeration
* SMB
* LDAP
* Initial access

### Hands-On Actions

* Enumerated Active Directory services
* Identified domain information
* Enumerated users and groups
* Investigated available network services
* Collected information that could be used for further assessment

### Key Takeaways

* Enumeration is a critical stage of an AD security assessment
* Attackers can gather significant information before authenticating
* Excessive information exposure can assist attackers
* Network segmentation and proper access controls reduce attack surface

---

## 5. AD: Authenticated Enumeration

### Topics Covered

* Authenticated enumeration
* Domain users
* Groups
* Permissions
* Domain resources
* Active Directory reconnaissance

### Hands-On Actions

* Enumerated the domain using an authenticated account
* Investigated users and groups
* Reviewed available permissions
* Identified domain resources
* Analyzed information available to authenticated users

### Key Takeaways

* Authenticated users may have access to significant directory information
* Excessive permissions can increase the attack surface
* Least privilege is essential when assigning access
* Regular access reviews can identify unnecessary permissions

---

## 6. Intro to Credential Harvesting

### Topics Covered

* Credential storage
* Cached credentials
* Password exposure
* Credential theft
* Windows authentication artifacts

### Hands-On Actions

* Investigated how Windows stores credentials
* Examined credential caching
* Explored ways credentials can become exposed
* Identified potential credential harvesting opportunities
* Reviewed defensive strategies for protecting credentials

### Key Takeaways

* Credentials can exist in multiple locations throughout an environment
* Compromised credentials can lead to privilege escalation
* Credential exposure can enable lateral movement
* Privileged credentials should receive additional protection

---

## 7. Intro to AD Lateral Movement

### Topics Covered

* Lateral movement
* PsExec
* WinRM
* Pass-the-Hash
* SSH tunneling
* Remote administration

### Hands-On Actions

* Explored Windows remote administration techniques
* Used PsExec in the lab environment
* Investigated WinRM
* Examined Pass-the-Hash concepts
* Explored SSH tunneling and pivoting

### Key Takeaways

* Compromised credentials can allow attackers to move between systems
* Excessive administrative privileges increase lateral movement opportunities
* Remote administration protocols should be properly secured and monitored
* Network segmentation can limit attacker movement

---

# 🧠 Key Concepts Learned

### Active Directory

Centralized directory service used to manage identities, computers, authentication, and access within Windows environments.

### Kerberos

Ticket-based authentication protocol used by Active Directory to securely authenticate users and services.

### NTLM

Legacy Windows authentication protocol that can introduce additional security risks compared to Kerberos.

### Enumeration

The process of gathering information about users, systems, groups, services, and permissions.

### Password Spraying

Attempting a small number of common passwords against many accounts rather than repeatedly attacking one account.

### Credential Harvesting

Obtaining usernames, passwords, hashes, tokens, or other authentication material.

### Lateral Movement

Moving from one compromised system or account to another within a network.

### Pass-the-Hash

An attack technique where an attacker uses a captured password hash to authenticate without knowing the original password.

### Least Privilege

Providing users and accounts only the permissions required to perform their assigned responsibilities.

---

# 🌍 Real-World Application

Active Directory is widely used in enterprise environments to manage identity, authentication, authorization, and access.

Security weaknesses in Active Directory can result in:

* Account compromise
* Privilege escalation
* Credential theft
* Unauthorized access
* Lateral movement
* Domain compromise

Understanding how attackers enumerate and exploit AD environments helps security professionals identify and remediate weaknesses before they can be abused.

These concepts are directly relevant to:

* Identity & Access Management (IAM)
* SOC Analyst
* Cybersecurity Analyst
* Security Engineer
* Active Directory Administrator
* Cloud Identity / Microsoft Entra ID

---

# ⚠️ Challenges Faced

* Understanding the relationship between Active Directory components
* Understanding Kerberos and NTLM authentication
* Learning different AD enumeration techniques
* Understanding how credentials can be exposed
* Understanding how compromised credentials enable lateral movement
* Connecting offensive techniques to defensive IAM controls

---

# ✅ How I Solved Them

* Broke each AD concept down into individual components
* Performed enumeration within the lab environment
* Practiced identifying users, groups, permissions, and services
* Compared different authentication mechanisms
* Documented attack techniques and their security implications
* Connected offensive techniques to defensive concepts such as MFA, least privilege, monitoring, and access reviews

---

# 📸 Screenshots

Screenshots documenting the lab environment and completed exercises are stored in the `/Screenshots` directory.

### Screenshots Include

* Active Directory enumeration
* Authentication testing
* User and group discovery
* Credential-related activities
* Lateral movement exercises
* Command-line tools and results

---

# 🧱 Lab Environment

* **Platform:** TryHackMe
* **Environment:** Windows Active Directory
* **Operating System:** Windows
* **Network:** Simulated Enterprise AD Environment

### Tools & Technologies

* Active Directory
* Windows
* PowerShell
* SMB
* LDAP
* Kerberos
* NTLM
* PsExec
* WinRM
* SSH
* Command Line

---

# 🎯 Skills Demonstrated

* Active Directory Security
* Active Directory Enumeration
* Identity & Access Management (IAM)
* Authentication
* Authorization
* Credential Security
* Privilege Management
* Network Enumeration
* Lateral Movement
* Windows Security
* PowerShell
* Security Assessment
* Least Privilege
* Enterprise Identity Security

---

# 🔗 Lab Link

[TryHackMe – Active Directory Security Testing Basics](https://tryhackme.com/module/active-directory-security-testing-basics)

---

# 🚀 Next Steps

* Continue practicing Active Directory enumeration
* Build a personal Windows Active Directory lab
* Practice BloodHound for AD relationship mapping
* Expand into Active Directory hardening
* Practice detecting AD attacks using SIEM tools
* Continue developing Microsoft Entra ID skills
* Practice Privileged Identity Management (PIM)
* Explore hybrid identity environments
* Continue toward IAM and Cloud Security roles

---

# 📌 Summary

This project demonstrates hands-on experience with **Active Directory security testing**, including authentication, enumeration, credential security, and lateral movement.

The lab strengthened my understanding of how identity and access weaknesses can be exploited in enterprise environments and how security controls such as **least privilege, MFA, monitoring, and proper access management** can reduce those risks.

This project serves as a foundation for further development in **Identity & Access Management, Microsoft Entra ID, Privileged Identity Management, and Cloud Security.**

