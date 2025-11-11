# 🛡️ Microsoft 365 Security Hardening Project

This project documents the end-to-end implementation of a secure Microsoft 365 tenant aligned with **CIS Benchmarks** and **Zero Trust principles**.

## 🎯 Objectives
- Build a secure M365 tenant from scratch
- Document configurations with rationale
- Map to CIS Benchmarks and best practices
- Automate security and compliance enforcement

## 🧩 Areas Covered
- Entra ID (Azure AD)
- Intune Device Management
- Microsoft Defender Suite
- CIS Benchmark Validation
- Automation via Graph, Power Automate, Sentinel

## 📊 Progress Tracker
| Area | Status | Notes |
|------|---------|-------|
| Entra ID | 🚧 In Progress | Conditional Access and RBAC done |
| Intune | 🚧 In Progress | Patch Rings & Compliance pending |
| Defender | 🚧 In Progress | MDE Configured, MDCA Integration next |

## 💬 Collaboration
Open a discussion or connect on [LinkedIn](https://linkedin.com/in/nathaniel-spencer-133903153)


## 👥 The Tenant Setup

### 🔹 Demo Users
- **Created 25 demo users** for testing and simulation.
- Bulk-created users via CSV import and onboarded them into **Entra ID**.
- Used PowerShell automation to streamline the process.

<img width="940" height="684" alt="image" src="https://github.com/user-attachments/assets/fa698229-b00b-4729-a0c8-0bc79307af80" />


### 🔹 User Settings
- Configured **user security settings** to align with **Zero Trust principles**.  

<img width="936" height="804" alt="image" src="https://github.com/user-attachments/assets/881d581a-74fe-43f8-acab-7b7e17627f76" />
<img width="904" height="723" alt="image" src="https://github.com/user-attachments/assets/fb253e7e-848f-4f2e-8100-37cb8916d17c" />


### 🔹 Custom Branding
- Implemented **custom branding** in Entra ID login pages.  
  This reduces phishing risk by helping users visually confirm legitimate login portals.

<img width="1290" height="641" alt="image" src="https://github.com/user-attachments/assets/d7aba0f1-2713-4417-a606-0c2d8668a94d" />


### 🔹 Dynamic Groups
- Created a **Dynamic Group** including all employee accounts for simplified management and automation.

<img width="814" height="587" alt="image" src="https://github.com/user-attachments/assets/4c46be19-6531-4d76-abd9-773c1fad34ad" />


### 🔹 Session Timeout
- Configured **idle session timeout** to **45 minutes** to reduce exposure from inactive sessions.

### 🔹 Licensing
- Established a **Group-Based Licensing Policy**:  
  - All members of the “All Company” group automatically receive **Microsoft 365 Business Premium** licenses.

### 🔹 Mock Groups
- Created **mock organizational groups** for policy scoping and testing:
  - `IT_Admins`
  - `HR_Team`
  - `Finance_Department`
  - `Executives`

### 🔹 Password Management
- **Reset all user passwords** using a PowerShell script for consistent lab access.  
- Script used: [`BulkPasswordChange.ps1`](../05_Automation/graph_api_scripts/BulkPasswordChange.ps1)  
- Documented all credentials securely for reference during testing.

---

> 🧠 **Note:** These configurations lay the foundation for identity hygiene, Zero Trust enforcement, and future Conditional Access and compliance testing.

