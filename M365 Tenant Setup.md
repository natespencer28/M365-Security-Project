## 👥 M365 Tenant Setup

### 🔹 Demo Users
- **Created 25 demo users** for testing and simulation.
- Bulk-created users via CSV import and onboarded them into **Entra ID**.
- Used PowerShell automation to streamline the process.

<img width="940" height="684" alt="image" src="https://github.com/user-attachments/assets/fa698229-b00b-4729-a0c8-0bc79307af80" />


### 🔹 User Settings
- Configured **user security settings** to align with **Zero Trust principles**.  

<img width="936" height="804" alt="image" src="https://github.com/user-attachments/assets/881d581a-74fe-43f8-acab-7b7e17627f76" />
<img width="904" height="723" alt="image" src="https://github.com/user-attachments/assets/fb253e7e-848f-4f2e-8100-37cb8916d17c" />

- Disabled Security Defaults and enabled Conditional Access policies regarding MFA

<img width="909" height="405" alt="image" src="https://github.com/user-attachments/assets/d79874ee-ed43-4a5b-b140-a605313daf5c" />


### 🔹 Custom Branding
- Implemented **custom branding** in Entra ID login pages.  
  This reduces phishing risk by helping users visually confirm legitimate login portals.

<img width="1290" height="641" alt="image" src="https://github.com/user-attachments/assets/d7aba0f1-2713-4417-a606-0c2d8668a94d" />


### 🔹 Dynamic Groups
- Created a **Dynamic Group** including all employee accounts for simplified management and automation.

<img width="814" height="587" alt="image" src="https://github.com/user-attachments/assets/4c46be19-6531-4d76-abd9-773c1fad34ad" />


### 🔹 Session Timeout
- Configured **idle session timeout** to **45 minutes** to reduce exposure from inactive sessions.
- (Will configure other Conditional Access policies for sign-in frequency and persistant browswer sessions in other documentation...)

### 🔹 Licensing
- Established a **Group-Based Licensing Policy**:  
  - All members of the “All Company” group automatically receive **Microsoft 365 Business Premium** licenses.

### 🔹 Mock Groups
- Created **mock organizational groups** for policy scoping and testing:

 <img width="309" height="263" alt="image" src="https://github.com/user-attachments/assets/3e470fe1-3549-4ee3-b678-673d2c05380d" />


### 🔹 Password Management
- **Reset all user passwords** using a PowerShell script for consistent lab access.  
- Script used: [`BulkPasswordChange.ps1`](../05_Automation/graph_api_scripts/BulkPasswordChange.ps1)

<img width="1025" height="1006" alt="Updateuserpasswords" src="https://github.com/user-attachments/assets/9b62cd25-db3a-401b-8172-a2a0f8846788" />

- Documented all credentials securely for reference during testing.
- Configured SSPR as well for self-service password resets.

<img width="387" height="188" alt="image" src="https://github.com/user-attachments/assets/369048cc-f8d6-403a-a4bc-f085967a342a" />

<img width="388" height="165" alt="image" src="https://github.com/user-attachments/assets/c9b5197c-a523-4864-bb7c-7151a1dbca91" />

  

---

> 🧠 **Note:** These configurations lay the foundation for identity hygiene, Zero Trust enforcement, and future Conditional Access and compliance testing.
