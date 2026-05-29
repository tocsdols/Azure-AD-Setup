# Azure-AD-Setup
# This project demonstrates the deployment of an Active Directory environment using Microsoft Azure and Windows Server. The lab simulates enterprise domain administration and user management.

##  Objectives:

• Deploy a Windows Server virtual machine in Azure
• Install Active Directory Domain Services (AD DS)
• Configure a domain controller
• Simulate enterprise user management

##  Skills Demonstrated:

• Active Directory Administration
• Azure Virtual Machine Deployment
• Windows Server Configuration
• User Account Management
• Group Policy Configuration
• Troubleshooting

##  Technologies Used:

• Microsoft Azure
• Windows Server 2025 Datacenter - x64 Gen2
• Active Directory Domain Services
• Windows 10 Client VM

##  Lab Environment

• Azure-hosted Windows Server acting as Domain Controller
• Windows client machine joined to the domain
• Domain Name: BENX.local

##  Implementation Summary:

1. Created a Windows Server VM in Azure
2. Installed Active Directory Domain Services
3. Promoted the server to a Domain Controller
4. Created Organizational Units and user accounts
5. Joined a client machine to the domain
6. Tested domain authentication

## Screenshots & Explanation

# PROJECT 1 — Azure AD Setup

_Created a Resource Group, a container where my virtual machines and Virtual Networks will be inside and named it LAB_RG_
<img width="1403" height="842" alt="image" src="https://github.com/user-attachments/assets/854c55a8-3239-4446-a588-0de4ade45115" />

_Created my Virtual Network (Vnet_Samuel) and added 2 subnets to it, which were later linked to my windows server and windows 10 VM_
<img width="1466" height="806" alt="image" src="https://github.com/user-attachments/assets/316c3aa3-5486-4395-99ba-b4f85d10cefc" />

_Created a Windows Server virtual machine in Microsoft Azure to serve as the Domain Controller for the Active Directory lab environment_
<img width="1459" height="824" alt="image" src="https://github.com/user-attachments/assets/8deba712-3c2a-4c2c-9a29-05e417fe4294" />
<img width="1336" height="716" alt="image" src="https://github.com/user-attachments/assets/8e8b3097-a2ea-45aa-82e3-f761ef1e0eab" />

_Initial Windows Server environment after deployment and configuration in Azure_
<img width="1460" height="829" alt="image" src="https://github.com/user-attachments/assets/eb9b3b9e-45c1-497c-939e-774abf02ccfb" />

_Installed Active Directory Domain Services (AD DS) role to enable domain management capabilities_
<img width="1332" height="814" alt="image" src="https://github.com/user-attachments/assets/a345a8bd-f983-4430-a08f-7bfa7f44eda6" />

_Promoted the Windows Server instance to a Domain Controller and configured a new domain environment_
<img width="1333" height="815" alt="image" src="https://github.com/user-attachments/assets/62cb109b-f007-4dad-99ae-fbbbd3aab313" />
<img width="1329" height="822" alt="image" src="https://github.com/user-attachments/assets/665125dc-e2b6-484e-bf20-29589d95a580" />

_Verified successful Active Directory deployment and access to domain management tools_
<img width="1332" height="828" alt="image" src="https://github.com/user-attachments/assets/9f62bc98-6275-4bb1-8c02-2496ed6be5c0" />

_Logging in the Windows Server 2025 Datacenter through the Windows App and showing the windows 10 VM active state_
<img width="1463" height="831" alt="image" src="https://github.com/user-attachments/assets/8f6e4dbf-cae3-4e1d-a412-3fb848ca2e83" />
<img width="1326" height="835" alt="image" src="https://github.com/user-attachments/assets/86c21658-b325-4a03-9ddb-8ef7b0ed2492" />

_Promoting Windows 10 VM to BENX.local DC windows Server DC 2025_
<img width="1328" height="817" alt="image" src="https://github.com/user-attachments/assets/98a7d116-9a2a-4a93-965b-43bcc191b5bf" />
<img width="1329" height="827" alt="image" src="https://github.com/user-attachments/assets/f34674f0-700c-4642-8064-c8a125173a35" />




# PROJECT 2 — User Administration

_Created domain user accounts and assigned them to appropriate departments and security groups_
<img width="1326" height="827" alt="image" src="https://github.com/user-attachments/assets/a56f2b01-d295-430a-ab2a-7dc42032cc46" />

_Created Organizational Units (OUs) to simulate departmental structure within an enterprise environment_
<img width="1330" height="823" alt="image" src="https://github.com/user-attachments/assets/79d614bd-9c26-4d59-96d7-4df1abde4e8a" />

_Configured security groups to support role-based access control and permission management_
<img width="1325" height="824" alt="image" src="https://github.com/user-attachments/assets/eb4bcb3e-c1c7-4fb8-be1d-a79050a9e925" />
<img width="1328" height="832" alt="image" src="https://github.com/user-attachments/assets/849309a2-eaed-4750-b936-580760c4ae61" />

_Configured password and account lockout policies using Group Policy Management_


_Configured and deployed dual Active Directory Group Policy Objects (GPOs) using security filtering for the Engineering Organizational Unit (OU)._

_Policy 1 (Enforcement): Configured Desktop Wallpaper policy to force a designated corporate background image_
_Policy 2 (Restriction): Enabled Prevent changing desktop background to lock down user personalization settings_

<img width="1326" height="830" alt="image" src="https://github.com/user-attachments/assets/c1362a46-29eb-49c3-9f0c-efbb320ee740" />
<img width="1324" height="826" alt="image" src="https://github.com/user-attachments/assets/f85dc825-fb24-439a-810f-efc44895215c" />
<img width="1324" height="825" alt="image" src="https://github.com/user-attachments/assets/ab8358af-86d4-4343-bad6-caa2113eaa65" />
<img width="1324" height="823" alt="image" src="https://github.com/user-attachments/assets/c828a7c2-da3f-41ac-bd17-81b591deed9d" />

Account Lockout
_Simulated account lockout scenario and restored user access through Active Directory account management_
<img width="1329" height="826" alt="image" src="https://github.com/user-attachments/assets/f6c17303-87ce-4732-9a15-d2fe55e0291e" />
<img width="1163" height="679" alt="image" src="https://github.com/user-attachments/assets/3e4c3d9c-2af6-4b46-b52a-07fe78012f72" />

_Performed password reset for a domain user account as part of standard Helpdesk support procedures_
<img width="1329" height="815" alt="image" src="https://github.com/user-attachments/assets/9cdc84b5-0ab8-4dab-8fb0-1bef127029de" />






























## 🎥 Project Demo

Watch the full project walkthrough and live demonstration here:

[YouTube Demo Link](https://www.youtube.com/watch?v=yJuEgMhqsNk)













