# active-directory-homelab

# 🔐 Active Directory Domain Services (AD DS) Homelab

Enterprise Active Directory deployment and configuration using Windows Server 2019 and Windows 10 clients in a virtualized lab environment.

---

## 📌 Project Overview

This project demonstrates the complete deployment and configuration of an Active Directory Domain Services (AD DS) environment using Windows Server 2019 and Windows 10 client machines. The lab was built in an isolated virtualized environment using VirtualBox/VMware to simulate a real-world enterprise network.

The project includes Domain Controller installation, DNS configuration, Organizational Unit (OU) management, user and group administration, client domain joining, authentication testing, and troubleshooting.

---

## 🎯 Lab Objectives

* Install and configure Windows Server 2019
* Configure a static IP address and DNS settings
* Install Active Directory Domain Services (AD DS)
* Promote the server to a Domain Controller
* Create a new forest and domain: `cyberlab_aj.local`
* Configure Organizational Units (OUs)
* Create and manage domain users and groups
* Join Windows 10 clients to the domain
* Verify authentication and permissions
* Perform troubleshooting and validation

---

# 🖥️ Lab Environment

| Component         | Details                       |
| ----------------- | ----------------------------- |
| Domain Name       | cyberlab_aj.local             |
| Domain Controller | DC01                          |
| Server OS         | Windows Server 2019           |
| Client OS         | Windows 10                    |
| Network           | 192.168.10.0/24               |
| DC IP Address     | 192.168.10.1                  |
| Client IPs        | 192.168.10.10 / 192.168.10.12 |
| Virtualization    | VirtualBox / VMware           |

---

# 🛠️ Technologies Used

* Active Directory Domain Services (AD DS)
* DNS
* DHCP
* Group Policy
* RSAT Tools
* Windows Server 2019
* Windows 10
* VirtualBox / VMware
* PowerShell

---

# 🌐 Network Architecture

```text
                 +----------------------+
                 |  Windows 10 Client   |
                 |      CLIENT01        |
                 +----------+-----------+
                            |
                            |
                    192.168.10.0/24
                            |
                            |
                 +----------+-----------+
                 | Domain Controller    |
                 | Windows Server 2019  |
                 | DC01                 |
                 | AD DS + DNS + DHCP   |
                 +----------------------+
```

---

# ⚙️ Key Tasks Performed

## ✅ Windows Server Configuration

* Installed Windows Server 2019
* Configured static IP addressing
* Configured DNS settings
* Verified network connectivity

## ✅ Active Directory Deployment

* Installed the AD DS role
* Promoted the server to a Domain Controller
* Created a new forest: `cyberlab_aj.local`
* Configured DNS integration

## ✅ User & Group Management

* Created Organizational Units (OUs)
* Created domain users and groups
* Added users to security groups
* Verified group membership

## ✅ Client Domain Join

* Configured Windows 10 client DNS
* Joined Windows clients to the domain
* Verified Kerberos authentication
* Tested domain logins

## ✅ Troubleshooting & Validation

* Used `ping`, `nslookup`, and `ipconfig`
* Verified DNS resolution
* Checked AD object registration
* Validated authentication and connectivity

---

# 📸 Screenshots

## Server Manager Dashboard
<img width="1022" height="730" alt="2" src="https://github.com/user-attachments/assets/1a61c220-380f-468e-bc8c-7d38b65c52b8" />

## AD DS Installation
<img width="762" height="562" alt="22" src="https://github.com/user-attachments/assets/5e784c43-688c-4d62-8511-1be22e21b37c" />

## Domain Controller Promotion

<img width="877" height="702" alt="45" src="https://github.com/user-attachments/assets/ccad29db-0325-49b0-b472-d2068c060d7f" />

## Active Directory Users and Computers

<img width="756" height="606" alt="47" src="https://github.com/user-attachments/assets/ee211ffa-1d7a-4405-abeb-1029cc26620f" />

## Domain Join Success

<img width="327" height="212" alt="32" src="https://github.com/user-attachments/assets/8d95610b-fde5-4e52-89b9-aee62e1f8682" />

---
# Miscellaneous
<img width="1890" height="757" alt="50" src="https://github.com/user-attachments/assets/3f9b6e85-bb3f-4da0-8792-e94f1b041cef" />

<img width="1893" height="712" alt="52" src="https://github.com/user-attachments/assets/5ca00e96-6beb-4aef-b98e-04aa085e384f" />

<img width="797" height="580" alt="27" src="https://github.com/user-attachments/assets/f82aef20-bb96-427f-a996-03b96089c76c" />


# 📚 Skills Demonstrated

* Active Directory Administration
* Windows Server Management
* DNS Configuration
* Domain Management
* User & Group Administration
* Identity & Access Management
* Enterprise Authentication
* Troubleshooting & Validation
* Virtualization & Networking

---

# 🔍 Useful Commands

```powershell
ipconfig /all
ping 192.168.10.1
nslookup cyberlab_aj.local
whoami
net user /domain
gpupdate /force
dcdiag
repadmin /showrepl
```

# 🚀 Future Improvements

* Configure Group Policy Objects (GPOs)
* Implement SIEM monitoring with Splunk
* Automate tasks using PowerShell
* Add additional domain clients
* Create a multi-domain forest environment
* Implement Active Directory security auditing

# 💡 Key Concepts Learned

| Concept              | Description                                  |
| -------------------- | -------------------------------------------- |
| AD DS                | Centralized authentication and authorization |
| DNS                  | Name resolution for domain services          |
| Domain Controller    | Server managing authentication and policies  |
| Kerberos             | Authentication protocol used in AD           |
| Organizational Units | Containers for organizing AD objects         |
| Security Groups      | Permission management for users              |
| Group Policy         | Centralized system configuration management  |

---

# 👨‍💻 Author

**Ajaj Ahmed**

Cybersecurity Enthusiast | SOC Analyst Learner | Windows Server & Active Directory Homelab Builder


# ⭐ Project Status

✅ Completed and Successfully Tested

