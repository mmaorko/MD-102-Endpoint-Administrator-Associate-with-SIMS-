🧭 1. Core Understanding of MD-102

Exam MD-102 covers four main domains:
| Section                                   | Weight | Focus                                                  |
| ----------------------------------------- | ------ | ------------------------------------------------------ |
| 1️⃣ Deploy Windows Client                 | 25–30% | Installation, configuration, and image deployment      |
| 2️⃣ Manage Identity and Compliance        | 15–20% | Azure AD, Intune policies, conditional access          |
| 3️⃣ Manage, Maintain, and Protect Devices | 40–45% | Intune, device configuration, Windows Update, Defender |
| 4️⃣ Manage Apps                           | 10–15% | App deployment, policies, Store apps, Win32 apps       |



2. Everyday & Must-Know Topics

These are the practical, everyday tasks that a Microsoft Endpoint Administrator performs:

🔹 A. Microsoft Intune (Endpoint Manager)

(This is the heart of MD-102 and daily work)
You should be confident in:

Device enrollment methods:

Azure AD Join

Hybrid Azure AD Join

Autopilot setup

BYOD (Bring Your Own Device)

Configuration profiles:

Wi-Fi, VPN, email, and security baselines

Compliance policies:

Device health, encryption, password, OS version rules

Conditional Access:

Integration with Azure AD security

Windows Update for Business (WUfB)

Remote actions:

Wipe, retire, sync, locate, lock device

📅 Used Daily: Intune portal (https://intune.microsoft.com
)

🔹 B. Azure Active Directory (now Entra ID)

Device join types (Azure AD Join, Hybrid)

User and group management

Role-based access control (RBAC)

Device registration and lifecycle

Conditional Access + MFA policies

Enterprise mobility integration with Intune

📅 Used Daily: Entra admin center (https://entra.microsoft.com
)

🔹 C. Windows Autopilot

Understanding Autopilot profiles

Setup and configuration process

Deployment modes:

User-driven, Self-deploying, Pre-provisioned

Troubleshooting deployment issues

📅 Used Often: When onboarding new devices

🔹 D. Windows Configuration and Updates

Local vs Intune policy precedence

Windows Update for Business configuration

Feature update rings and deployment schedules

Troubleshooting updates and rollback

📅 Used Weekly: Maintaining device patch compliance

🔹 E. Security & Protection

Microsoft Defender for Endpoint integration

BitLocker device encryption management

Compliance policy enforcement

Attack surface reduction (ASR) rules

Endpoint security configuration in Intune

📅 Used Daily: Ensuring devices are secure and compliant

🔹 F. Application Management

App deployment types:

Win32, Microsoft Store, Office, LOB apps

Deployment assignment (required/available/uninstall)

App protection policies (for MAM)

WinGet and Winget-cli basics

📅 Used Daily: Installing or updating user apps remotely

🔹 G. Troubleshooting & Monitoring

Intune device troubleshooting pane

Event Viewer, logs, and diagnostic data

Endpoint analytics (performance, boot time)

Policy conflicts and compliance status

Remote assist and device diagnostics

📅 Used Daily: Supporting end-users and resolving device issues

🧰 3. Tools You Should Know
| Tool                                 | Purpose                    |
| ------------------------------------ | -------------------------- |
| **Intune Admin Center**              | Device management          |
| **Azure/Entra Admin Center**         | User & identity management |
| **Windows Admin Center**             | Local device management    |
| **PowerShell / Graph API**           | Automation                 |
| **Microsoft Endpoint Manager (MEM)** | Combined portal view       |
| **Event Viewer / CMD / PowerShell**  | Local troubleshooting      |


📚 4. Practice Topics for Certification

If preparing for the MD-102 exam, focus especially on:

Deploying Windows with Autopilot

Managing compliance and Conditional Access

Configuring device policies in Intune

Deploying and managing applications

Securing endpoints with Defender and BitLocker

Monitoring and reporting device compliance

🧩 5. Everyday Workflow Example

Here’s what a normal day might include for an Endpoint Admin:

Check Intune dashboard for compliance alerts

Approve or troubleshoot Autopilot deployments

Deploy a new Win32 app or update policy

Use Endpoint analytics for performance reports

Enforce security baselines and update rings

Respond to user tickets about device access or MFA
