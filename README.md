# Azure Active Directory Home Lab
# This project demonstrates the deployment of an Active Directory environment using Microsoft Azure and Windows Server. The lab simulates enterprise domain administration and user management.

##  Objectives:

• Deploy a Windows Server virtual machine in Azure
• Install Active Directory Domain Services (AD DS)
• Configure a domain controller
• Simulate enterprise user management

---

##  Skills Demonstrated:

• Active Directory Administration
• Azure Virtual Machine Deployment
• Windows Server Configuration
• User Account Management
• Group Policy Configuration
• Troubleshooting

---

##  Technologies Used:

• Microsoft Azure
• Windows Server 2025 Datacenter - x64 Gen2
• Active Directory Domain Services
• Windows 10 Client VM

---

##  Lab Environment

• Azure-hosted Windows Server acting as Domain Controller
• Windows client machine joined to the domain
• Domain Name: BENX.local

---

##  Implementation Summary:

1. Created a Windows Server VM in Azure
2. Installed Active Directory Domain Services
3. Promoted the server to a Domain Controller
4. Created Organizational Units and user accounts
5. Joined a client machine to the domain
6. Tested domain authentication

---

## Screenshots & Explanation

# PROJECT 1 — [Azure-AD-Deployment](https://github.com/tocsdols/Azure-AD-Deployment)

_Created a Resource Group, a container where my virtual machines and Virtual Networks will be inside and named it LAB_RG_
<img width="850" height="842" alt="image" src="https://github.com/user-attachments/assets/854c55a8-3239-4446-a588-0de4ade45115" />

_Created my Virtual Network (Vnet_Samuel) and added 2 subnets to it, which were later linked to my windows server and windows 10 VM_
<img width="850" height="806" alt="image" src="https://github.com/user-attachments/assets/316c3aa3-5486-4395-99ba-b4f85d10cefc" />

_Created a Windows Server virtual machine in Microsoft Azure to serve as the Domain Controller for the Active Directory lab environment_
<img width="850" height="824" alt="image" src="https://github.com/user-attachments/assets/8deba712-3c2a-4c2c-9a29-05e417fe4294" />
<img width="850" height="716" alt="image" src="https://github.com/user-attachments/assets/8e8b3097-a2ea-45aa-82e3-f761ef1e0eab" />

_Initial Windows Server environment after deployment and configuration in Azure_
<img width="850" height="829" alt="image" src="https://github.com/user-attachments/assets/eb9b3b9e-45c1-497c-939e-774abf02ccfb" />

_Installed Active Directory Domain Services (AD DS) role to enable domain management capabilities_
<img width="850" height="814" alt="image" src="https://github.com/user-attachments/assets/a345a8bd-f983-4430-a08f-7bfa7f44eda6" />

_Promoted the Windows Server instance to a Domain Controller and configured a new domain environment_
<img width="850" height="815" alt="image" src="https://github.com/user-attachments/assets/62cb109b-f007-4dad-99ae-fbbbd3aab313" />
<img width="850" height="822" alt="image" src="https://github.com/user-attachments/assets/665125dc-e2b6-484e-bf20-29589d95a580" />

_Verified successful Active Directory deployment and access to domain management tools_
<img width="850" height="828" alt="image" src="https://github.com/user-attachments/assets/9f62bc98-6275-4bb1-8c02-2496ed6be5c0" />

_Logging in the Windows Server 2025 Datacenter through the Windows App and showing the windows 10 VM active state_
<img width="850" height="831" alt="image" src="https://github.com/user-attachments/assets/8f6e4dbf-cae3-4e1d-a412-3fb848ca2e83" />
<img width="850" height="835" alt="image" src="https://github.com/user-attachments/assets/86c21658-b325-4a03-9ddb-8ef7b0ed2492" />

_Joined the Windows 10 client machine to the BENX.local Active Directory domain environment_
<img width="850" height="817" alt="image" src="https://github.com/user-attachments/assets/98a7d116-9a2a-4a93-965b-43bcc191b5bf" />
<img width="850" height="827" alt="image" src="https://github.com/user-attachments/assets/f34674f0-700c-4642-8064-c8a125173a35" />

---

# PROJECT 2 — [AD-User-Management](https://github.com/tocsdols/AD-User-Management)


## Outcome

Successfully deployed and configured an Active Directory environment in Microsoft Azure using Windows Server 2025. 

The project provided hands-on experience with:
- Domain administration
- User and group management
- Group Policy configuration
- Domain authentication
- Account lockout troubleshooting
- Password reset procedures

This lab strengthened foundational skills relevant to IT Support, System Administration, and Cybersecurity environments.

---

## Key Takeaways

- Learned how enterprise domain environments are structured
- Understood how Group Policy Objects affect users and systems
- Gained experience troubleshooting authentication and account lockout issues
- Improved familiarity with Azure networking and Windows Server administration




















