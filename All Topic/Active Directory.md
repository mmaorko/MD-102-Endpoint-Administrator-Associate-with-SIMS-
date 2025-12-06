# What is Active Directory (AD)?

Microsoft Active Directory (AD) is a directory service developed by Microsoft that is used for managing users, computers, and other resources on a network.
It acts like a centralized database where you can manage identities, permissions, and security settings across your organization.

![enter image description here](https://i.ibb.co.com/d4JxXkX3/2025-12-06-155150.png)

## what information is store on active directory?
🔐 User and Security Information
  - User accounts: Username, password hashes, group memberships, login scripts, home directories, etc.
  - Permissions and access control: Who can access what and at what level (through Access Control Lists).
💻 Computer and Device Information
  - Computer accounts: Info about machines joined to the domain.
  - Operating system details: OS version, service pack, etc.
  - Group Policy Objects (GPOs): Policies applied to computers or users (e.g., password rules, software deployment, etc.).
🌐 Network and Domain Services
  - Domains, Trees, and Forests: AD structures that define boundaries of administrative control and replication.
  - DNS information: Integration with DNS for locating services (e.g., domain controllers).
  - Sites and Subnets: Info used for optimizing replication and login traffic.
### Active Directory (AD) has a hierarchical structure that organizes and manages network resources efficiently. Here’s an overview of the main components of the Active Directory structure, from top to bottom:
![enter image description here](https://i.ibb.co/xS1y398B/2025-05-19-210629.png)

## Common task Active Directory 
- Create user accounts
- Reset passwords
- Unlock user accounts
- Disable or delete accounts
- Move users between Organizational Units (OUs)
- Update user attributes (e.g., job title, department, email)


## Important Topics Active Directory
1. 🧱 Active Directory Domain Services (AD DS)
Central service that handles authentication, directory storage, and access control.

Understand users, groups, OUs, domains, and trusts.

2. 🔐 User and Group Management
Creating, modifying, and deleting user and group accounts.

Understanding security vs. distribution groups.

Group nesting and permission inheritance.

3. 🖥️ Organizational Units (OUs) and Delegation
Structuring AD using OUs for administrative and policy purposes.

Delegating permissions using the Delegation of Control Wizard.

4. 🎯 Group Policy Objects (GPOs)
Creating and linking GPOs to enforce security, desktop, and software policies.

Group Policy inheritance, precedence, loopback, and troubleshooting.

5. 💻 Domain Controllers (DCs)
Role and function of DCs in authentication and replication.

Understanding FSMO roles, Read-Only Domain Controllers (RODCs), and Global Catalogs.

6. 🌐 Trusts and Forests
How domains trust each other in a multi-domain or multi-forest environment.

Types of trusts: transitive, non-transitive, one-way, two-way.

7. 🔄 Replication and Sites/Subnets
How AD replicates data across domain controllers.

Using Sites and Services to control replication traffic and authentication based on location.

8. 🧬 Schema and Global Catalog
AD schema defines object classes and attributes.

The Global Catalog enables forest-wide searches and authentication for universal groups.

9. 🧰 Backup, Recovery, and AD Maintenance
Backing up AD using Windows Server Backup.

Using Authoritative vs. Non-authoritative Restore.

Tools like ntdsutil, wbadmin.

10. ⚙️ PowerShell and Automation
Managing AD using PowerShell cmdlets (e.g., Get-ADUser, New-ADGroup, etc.).

Writing scripts to automate account creation, cleanup, reports, etc.





### 🧠 Core Components of AD Domain Services (AD DS)
| Component                  | Description                                                                 |
| -------------------------- | --------------------------------------------------------------------------- |
| **Domain Controller (DC)** | Server that runs AD DS and handles authentication and directory services    |
| **Global Catalog**         | Partial, read-only copy of all objects in the forest                        |
| **FSMO Roles**             | Flexible Single Master Operation roles that ensure proper functioning of AD |
| **Group Policies (GPO)**   | Centralized management of security settings, software deployment, scripts   |
| **Trusts**                 | Relationships between domains to share resources                            |


🛠️ Common Admin Tasks in AD Domains
| Task                           | Tool                                                |
| ------------------------------ | --------------------------------------------------- |
| Create/Manage users and groups | **Active Directory Users and Computers (ADUC)**     |
| Apply security settings        | **Group Policy Management Console (GPMC)**          |
| Monitor replication and health | **Active Directory Sites and Services**, `repadmin` |
| Backup/Restore AD              | Windows Server Backup, Veeam                        |
| Delegate permissions           | Use OUs and GPO delegation                          |
| Join computers to domain       | Via system properties or script (PowerShell)        |



### 💻 Important Tools & Commands
dsa.msc – Open ADUC (Active Directory Users & Computers)

gpmc.msc – Open Group Policy Management Console

dsadd, dsmod, dsquery – CLI tools to manage objects

netdom – Manage domain joins and trusts

repadmin – Monitor and troubleshoot AD replication

PowerShell – e.g., Get-ADUser, New-ADUser
