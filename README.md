# windows-active-directory-group-policy-lab
Windows Server Active Directory and Group Policy lab demonstrating OU structure, user/group management, GPO enforcement, and domain troubleshooting.
# Windows Server Active Directory & Group Policy Lab

## 📌 Project Overview

This project demonstrates the deployment and administration of a Windows Server Active Directory environment within Oracle VirtualBox. A Windows Server domain controller was configured to manage users, organizational units (OUs), security groups, and Group Policy Objects (GPOs). A Windows 11 client computer was joined to the domain to verify centralized authentication and policy enforcement.

This lab simulates common enterprise system administration tasks, including user and group management, organizational structure, Group Policy configuration, and troubleshooting domain connectivity.

## 🎯 Objectives

* Install and configure Active Directory Domain Services (AD DS)
* Create and manage Organizational Units (OUs)
* Create domain users and security groups
* Join a Windows 11 client to the Active Directory domain
* Configure and apply Group Policy Objects (GPOs)
* Verify Group Policy enforcement on a domain-joined client
* Troubleshoot domain authentication and network connectivity issues

## 🛠️ Technologies Used

* Windows Server
* Active Directory Domain Services (AD DS)
* Group Policy Management
* Windows 11
* Oracle VirtualBox
* DNS
* Active Directory Users and Computers (ADUC)
* Group Policy Objects (GPO)

## 🏗️ Lab Environment

| Component         | Configuration                       |
| ----------------- | ----------------------------------- |
| Hypervisor        | Oracle VirtualBox                   |
| Domain Controller | Windows Server                      |
| Client Machine    | Windows 11 Pro                      |
| Domain Name       | CORP.local                          |
| Primary Services  | Active Directory, DNS, Group Policy |
| Authentication    | Domain-based user authentication    |
| Network           | VirtualBox NAT Network              |

## 🚀 Lab Steps

### 1. Active Directory Installation

* Installed and configured Active Directory Domain Services (AD DS).
* Promoted the Windows Server to a Domain Controller.
* Created the **CORP.local** Active Directory domain.

### 2. Organizational Unit (OU) Creation

* Created Organizational Units (OUs) to organize users and administrative resources.
* Implemented a logical structure for IT, HR, and other organizational departments.

### 3. User and Security Group Management

* Created domain user accounts.
* Created security groups for administrative and departmental access.
* Assigned users to the appropriate security groups.

### 4. Windows 11 Domain Join

* Joined the Windows 11 client computer to the **CORP.local** domain.
* Verified successful domain authentication.

### 5. Group Policy Configuration

* Created and linked a Group Policy Object (GPO).
* Configured a policy to restrict access to Control Panel for standard users.
* Applied the policy to the appropriate Organizational Unit.

### 6. Group Policy Verification

* Forced a Group Policy update.
* Logged in as a standard domain user.
* Verified that the Control Panel restriction was successfully enforced.

### 7. Troubleshooting

* Diagnosed domain authentication failures caused by loss of DHCP connectivity.
* Verified DNS configuration and domain controller communication.
* Isolated the issue by assigning a temporary static IPv4 address.
* Restored successful domain authentication and validated Group Policy functionality.

## 📸 Screenshots

### Active Directory Users and Computers

![Active Directory](Screenshots/Active-Directory.PNG)

### Group Policy Management

![Group Policy Management](Screenshots/Group-Policy-Management.PNG)

### Group Policy Restriction Verification

![Restrictions](Screenshots/Restrictions-Message.png)

## 🎓 Skills Demonstrated

* Windows Server administration
* Active Directory Domain Services (AD DS)
* Organizational Unit (OU) management
* Domain user and security group administration
* Group Policy Object (GPO) creation and management
* Windows 11 domain integration
* DNS configuration and troubleshooting
* Enterprise authentication troubleshooting
* Network connectivity troubleshooting
* VirtualBox virtualization

## 💡 Key Takeaways

This project demonstrates foundational enterprise Windows administration by configuring an Active Directory environment, managing users and groups, deploying Group Policy, and validating centralized authentication. It also highlights practical troubleshooting skills by identifying and resolving domain connectivity issues related to network configuration, resulting in successful Group Policy enforcement on a domain-joined Windows 11 client.
