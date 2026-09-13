# IT Home Lab Portfolio

Welcome to my IT Home Lab Portfolio. This repository documents my hands-on experience with Windows Server, Active Directory, Group Policy, and Microsoft technologies as I build practical IT administration skills.

## Completed Labs

### Lab 01 - Active Directory Domain Setup
- Installed and configured Windows Server 2022
- Promoted DC01 to a Domain Controller
- Created the homelab.local Active Directory domain
- Joined a Windows 11 client to the domain

### Lab 02 - Group Policy Management
- Created and linked a Group Policy Object (GPO)
- Deployed a user policy across the domain
- Verified policy application using `gpupdate /force`

### Lab 03 - Active Directory User & Group Management
- Created and managed domain users
- Created and configured security groups
- Assigned users to appropriate groups
- Verified group membership and access

### Lab 04 - Group Policy Administration
- Created and configured additional Group Policy settings
- Linked and applied GPOs to domain users/computers
- Verified policy application on the Windows 11 client
- Troubleshot Group Policy configuration and application

### Lab 05 - Drive Mapping with Group Policy
- Created a Group Policy Object for Company Data drive mapping
- Configured Group Policy Preferences
- Mapped `\\DC01\CompanyData` to the S: drive
- Applied the policy using `gpupdate /force`
- Verified the mapped drive appeared automatically on CLIENT01
- Confirmed read/write access by creating a test file

## Skills Demonstrated

- Active Directory
- Group Policy Management
- Group Policy Preferences
- Windows Server 2022
- Windows 11 Administration
- User & Group Management
- Network Drive Mapping
- SMB File Sharing
- File & Folder Permissions
- Troubleshooting

## Upcoming Labs

- Password Policies & Account Lockouts
- DNS & DHCP
- File Shares & NTFS Permissions
- Active Directory Security Hardening
- Group Policy Security Filtering
- Active Directory Troubleshooting

## Current Progress

- ✅ Lab 01 Completed
- ✅ Lab 02 Completed
- ✅ Lab 03 Completed
- ✅ Lab 04 Completed
- ✅ Lab 05 Completed
- 🔨 Building additional Active Directory and Windows Server labs
