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
