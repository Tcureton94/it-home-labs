
# Lab 01 — Active Directory Domain Setup

## Objective

Build a functional Active Directory environment using Windows Server 2022, configure Active Directory Domain Services (AD DS) and DNS, join a Windows 11 client to the domain, and verify domain authentication and network connectivity.

## Lab Environment

| Component | Details |
|---|---|
| Hypervisor | VMware Workstation Pro |
| Domain Controller | DC01 |
| Client | CLIENT01 |
| Server OS | Windows Server 2022 |
| Client OS | Windows 11 Enterprise |
| Domain | homelab.local |

## Hands-On Tasks

- Installed Windows Server 2022
- Installed Active Directory Domain Services (AD DS)
- Promoted DC01 to a Domain Controller
- Created the `homelab.local` Active Directory domain
- Configured DNS
- Prepared and renamed a Windows 11 client to CLIENT01
- Configured CLIENT01 to use DC01 for DNS
- Joined CLIENT01 to the Active Directory domain
- Verified domain membership
- Created and verified a domain user account
- Verified Active Directory group membership
- Tested network connectivity and DNS name resolution

## Key Commands Used

```powershell
ipconfig
hostname
ping DC01
ping CLIENT01
whoami
```

## Screenshots
### Figure 1: Windows 11 Client ready for config.
<img width="1919" height="1079" alt="01  Windows 11 Client ready for config" src="https://github.com/user-attachments/assets/4cffbdda-35a3-495a-a13f-174f37b9b4ef" />

### Figure 2: installing VMware tools (windows 11 client)
<img width="1919" height="1070" alt="02  installing VMware tools (windows 11 client)" src="https://github.com/user-attachments/assets/ea055044-7f8f-48ba-85c8-0a7960e61583" />

### Figure 3: renaming windows 11 client to CLIENT01
<img width="1920" height="1080" alt="03  renaming windows 11 client to CLIENT01" src="https://github.com/user-attachments/assets/3ceda263-c0ee-468e-8f6b-9765e667bde9" />

### Figure 4: CLIENT01 DNS Configured to use DC01
<img width="1917" height="1079" alt="04  CLIENT01 DNS Configured to use DC01" src="https://github.com/user-attachments/assets/5b2add81-2825-43ad-95f6-4ea5ba6c0a43" />

### Figure 5: CLIENT01 Successfully resolves and pings DC01
<img width="1905" height="1069" alt="05  CLIENT01 Successfully resolves and pings DC01" src="https://github.com/user-attachments/assets/da0a6476-b9d3-4d26-a450-8cb627d9fa82" />

### Figure 6: CLIENT01 successfully joined homelab.local domain
<img width="1920" height="1080" alt="06  CLIENT01 successfully joined homelab local domain" src="https://github.com/user-attachments/assets/316088cd-fb29-4452-aed0-fb46b6bf4533" />

### Figure 7: CLIENT01 Domain Membership Verified
<img width="1920" height="1080" alt="07 CLIENT01 Domain Membership Verified" src="https://github.com/user-attachments/assets/aee6d818-9fb7-4423-8e54-1bf202ae6696" />

### Figure 8: Verified Mike Davis domain account with prompt whoami
<img width="1920" height="1080" alt="08  Verified Mike Davis domain account with prompt whoami" src="https://github.com/user-attachments/assets/3600b306-0f80-4999-ade8-5911b8c3d975" />

### Figure 9: Mike Davis Group Membership Verification
<img width="1920" height="1080" alt="09  Mike Davis Group Membership Verification" src="https://github.com/user-attachments/assets/467fd0f4-d308-418c-b696-b5a324172aa0" />


