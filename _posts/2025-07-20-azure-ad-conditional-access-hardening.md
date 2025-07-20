---
title: "Hardening Azure AD with Conditional Access & MFA"
excerpt: "Implemented Conditional Access and MFA controls to protect an Azure AD tenant against phishing and session hijack attacks."
layout: single
date: 2025-07-20
author_profile: true
tags: [Azure, IAM, Security, Conditional Access, MFA, Identity Protection]
---

## 🔐 Project: Azure AD Conditional Access Hardening

### 👨‍💻 Role
Cloud Security Engineer (Personal Lab)

### 🎯 Goal
To implement real-world **identity security controls** using Azure AD Conditional Access policies and MFA enforcement to mitigate common attacks like phishing, token theft, and impossible travel scenarios.

---

## 🛠️ Tools & Tech
- **Azure AD Free & Premium P1**
- **Microsoft Entra**
- **Microsoft Graph (via CLI)**
- **Admin accounts + test users**
- **Security defaults / custom Conditional Access**
- **PowerShell (AzureAD module)**

---

## 🧪 What I Did

- Enabled **Security Defaults**, then escalated to **custom Conditional Access policies** for better control.
- Created test scenarios using:
  - Impossible travel detection (Kenya to Germany simulation)
  - Risky sign-in alerts
  - Blocking legacy authentication (SMTP, POP3, IMAP)
- Implemented **MFA enforcement** for admin roles, and **location-based controls** (e.g., allow logins only from Kenyan IP ranges).
- Ran policy simulations to ensure minimal disruption during rollout.
- Documented impact using screenshots and sign-in logs.

---

## 💡 What I Learned

- How Conditional Access policies can **reduce attack surfaces** dramatically when configured well.
- Why blocking legacy authentication is **one of the most impactful hardening steps** in Azure.
- How to use **Microsoft Graph API & logs** to audit access attempts and fine-tune policy coverage.

---

## 📸 Screenshots
Add screenshots in your `/assets/images/` folder and link here:

```markdown
![Policy Simulation](../assets/images/ca-policy-simulation.png)
![User Blocked](../assets/images/mfa-blocked-user.png)
