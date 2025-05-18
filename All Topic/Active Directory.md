# What is Active Directory (AD)?

Microsoft Active Directory (AD) is a directory service developed by Microsoft that is used for managing users, computers, and other resources on a network.
It acts like a centralized database where you can manage identities, permissions, and security settings across your organization.

🧩 Key Concepts in Active Directory
1. 🏢 Domain
A domain is the core unit of AD—it groups objects like users, computers, and printers under a common security boundary.

Example: company.local or example.com

2. 🌍 Forest
A forest is the top-level container in AD that can contain multiple domains.

All domains in a forest trust each other and share a common schema and global catalog.

3. 🌲 Tree
A tree is a group of domains that share a contiguous namespace.

For example: hr.company.com, sales.company.com are part of the same tree under company.com.

4. 📁 Organizational Units (OUs)
Sub-containers inside domains used to organize and manage resources.

You apply Group Policies and permissions at the OU level.

5. 👤 Objects
Everything in AD is an object—users, groups, computers, printers, etc.

Each object has attributes (e.g., a user has name, email, group memberships).

🔐 Authentication & Authorization
✅ Authentication
Verifying who a user is (e.g., username/password).

Uses protocols like Kerberos or NTLM.

✅ Authorization
Determining what that user can access.

Managed through permissions and Group Policy Objects (GPOs).

🧠 Core Components of AD Domain Services (AD DS)
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

💻 Important Tools & Commands
dsa.msc – Open ADUC (Active Directory Users & Computers)

gpmc.msc – Open Group Policy Management Console

dsadd, dsmod, dsquery – CLI tools to manage objects

netdom – Manage domain joins and trusts

repadmin – Monitor and troubleshoot AD replication

PowerShell – e.g., Get-ADUser, New-ADUser
