🔹 What is Windows MDT?

MDT = Microsoft Deployment Toolkit

MDT is a free Microsoft tool used by IT admins to deploy Windows operating systems automatically in an organization.

✅ What MDT is used for

- Deploy Windows 10 / Windows 11

- Automate OS installation (no manual setup)

- Install drivers, applications, updates

- Join PCs to Active Directory

- Apply basic configurations

🛠 How MDT works (simple)

1. Import Windows image

2. Create Task Sequences

3. Add apps & drivers

4. Boot PC via PXE or USB

5. Windows installs automatically


🔹 What is Windows ADK?

ADK = Windows Assessment and Deployment Kit

ADK is a set of tools required to create, customize, and deploy Windows images.

✅ What ADK provides

- Windows PE (Preinstallation Environment)

- DISM (image servicing)

- USMT (User State Migration Tool)

⚠️ ADK does NOT deploy Windows by itself
It only provides the tools that other solutions (MDT, SCCM, WDS) use.

🔁 ADK Workflow (Real Deployment Flow)

- PC boots into Windows PE

- Disk is prepared

- DISM applies Windows image

- Windows setup runs using Unattend.xml

- Optional: USMT restores user data

- First boot into Windows

I- maging & deployment tools

👉 MDT cannot work without ADK

🧩 How MDT + ADK work together

- ADK provides the core tools

- MDT uses those tools to create a full deployment solution

📌 Think like this:

- ADK = Engine
- MDT = Car body + steering
