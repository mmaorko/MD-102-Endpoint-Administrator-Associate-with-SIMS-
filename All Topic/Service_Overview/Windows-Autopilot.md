1️⃣ Windows Autopilot কী?

Windows Autopilot হলো একটি Cloud-based device deployment solution
যার মাধ্যমে নতুন বা রিসেট করা Windows PC স্বয়ংক্রিয়ভাবে কনফিগার হয়।

📌 IT Admin কোনো ইমেজ বানায় না
📌 ইউজার শুধু সাইন-ইন করে
📌 বাকি সব কাজ ক্লাউড থেকে হয়

2️⃣ Windows Autopilot কেন ব্যবহার করা হয়?
| সমস্যা (Traditional) | সমাধান (Autopilot)   |
| -------------------- | -------------------- |
| Manual Windows setup | Automatic setup      |
| USB / Image দরকার    | Internet হলেই যথেষ্ট |
| Onsite IT দরকার      | Remote deployment    |
| সময় বেশি লাগে        | দ্রুত ডিভাইস রেডি    |

3️⃣ Windows Autopilot Architecture
New PC
  ↓
Internet
  ↓
Microsoft Entra ID
  ↓
Intune (MDM)
  ↓
Autopilot Profile
  ↓
Apps + Policies + Security

4️⃣ Windows Autopilot Setup (Step-by-Step)
Step 1️⃣ Device Hardware Hash Collect
Get-WindowsAutopilotInfo.ps1
Step 2️⃣ Upload Device in Intune

📍 Intune → Devices → Windows → Autopilot

Step 3️⃣ Create Autopilot Profile

- Deployment mode

- Join type (Entra / Hybrid)

- OOBE settings

Step 4️⃣ Assign Profile

- Assign to device group

Step 5️⃣ Reset / New Device Boot

- User sign-in → Auto configure


