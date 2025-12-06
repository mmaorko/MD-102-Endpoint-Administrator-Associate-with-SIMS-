1️⃣ Cloud Computing Basics

Microsoft-এর ক্লাউড সার্ভিস মূলত ৩টি মডেলে বিভক্ত—

✔ IaaS — Infrastructure as a Service

আপনার জন্য সার্ভার, নেটওয়ার্ক, স্টোরেজ ক্লাউডে তৈরি করে দেয়।
উদাহরণ: Azure Virtual Machine, VNet, Load Balancer

✔ PaaS — Platform as a Service

আপনার অ্যাপ চালানোর জন্য প্রস্তুত প্ল্যাটফর্ম দেয়।
উদাহরণ: Azure App Service, Azure SQL Database

✔ SaaS — Software as a Service

সম্পূর্ণ সফটওয়্যার রেডি অবস্থায় ব্যবহার করতে পারবেন।
উদাহরণ: Microsoft 365 (Outlook, Teams, OneDrive)

2️⃣ Shared Responsibility Model (অত্যন্ত গুরুত্বপূর্ণ)

Cloud provider (Microsoft) আর আপনি (Customer) দুজনেই দায়িত্ব ভাগাভাগি করেন।

Layer	Customer	Microsoft
SaaS	Data, Access	Software, Infra
PaaS	Apps, Config	OS, Infra
IaaS	OS, Apps, Data	Hardware
3️⃣ Microsoft Cloud-এর Core Building Blocks
✔ Microsoft Azure

Microsoft-এর Main Cloud Platform

Compute

Networking

Storage

Databases

Security

AI/ML

Azure = Public Cloud Foundation

✔ Microsoft Entra ID (Azure AD)

এটা হলো Cloud Identity Service—
মাইক্রোসফটের প্রতিটি ক্লাউড সার্ভিসে লগইন/অ্যাক্সেস ম্যানেজ করার “Identity Layer”।

Features:

Users / Groups

MFA

Conditional Access

SSO (Single Sign-On)

Device Identity

Entra ID ছাড়া Microsoft Cloud চলেই না।

✔ Microsoft 365

SaaS প্রোডাক্ট:

Exchange Online (Email)

SharePoint

OneDrive

Teams

Office Apps

এগুলো চালাতে Entra ID লাগে (Identity backbone)।

✔ Microsoft Intune

Device & App Management service:

Windows / Android / iOS device management

Compliance policies

App Deployment

Security Baselines

Endpoint Protection

Intune = MDM + MAM solution

✔ Microsoft Security Stack

Microsoft Defender for Endpoint

Defender for Identity

Defender for Office

Microsoft Sentinel (SIEM)

Purview (Compliance)

এগুলো Cloud Security Foundation তৈরি করে।

4️⃣ Global Infrastructure Basics

Microsoft Cloud বিশ্বব্যাপী চালানোর জন্য কয়েকটি ধারণা গুরুত্বপূর্ণ:

✔ Region

যেখানে Azure ডেটাসেন্টার অবস্থিত (উদাহরণ: East US, West Europe)

✔ Availability Zone

এক অঞ্চলের ভেতরে একাধিক ডেটাসেন্টার।
High availability নিশ্চিত করে।

✔ Tenant

আপনার প্রতিষ্ঠানের Microsoft Cloud identity boundary।
একটি tenant = একটি organization।

✔ Subscription

Azure resource এর billing container।
Tenant → Subscription → Resource group → Resources

5️⃣ Zero Trust Model

Microsoft Cloud-এর ভিত্তি নিরাপত্তা মডেল।

Principles:

Verify explicitly

Least privilege access

Assume breach

Intune + Entra ID + Defender = Zero Trust implementation tools.

🎯 You should master these 8 fundamentals:

Cloud computing (IaaS/PaaS/SaaS)

Shared responsibility model

Entra ID (Identity)

Azure basics (compute, networking, storage)

Microsoft 365 core

Intune fundamentals

Zero Trust security

Tenant structure (Tenant → Subscription → Resource Group → Resource)
