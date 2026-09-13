## Objective

Configure a Group Policy Object (GPO) to automatically map a shared network drive for domain users and verify that the mapped drive is available on a Windows 11 client after Group Policy is applied.

Environment

• Windows Server 2022 (DC01)
• Windows 11 Enterprise Client (CLIENT01)
• Active Directory Domain: homelab.local

What I Did

• Created a new Group Policy Object (GPO) named CompanyData Drive Mapping.
• Linked the GPO to the homelab.local domain.
• Configured a mapped network drive using Group Policy Preferences.
• Mapped the shared folder \\DC01\CompanyData to the S: drive.
• Assigned the drive label Company Data.
• Logged into CLIENT01 as a domain user.
• Applied Group Policy using gpupdate /force.
• Verified that the Company Data (S:) drive appeared automatically.
• Confirmed read and write access by creating a test file inside the mapped drive.

Results

Successfully deployed and verified a network drive mapping through Group Policy Preferences. CLIENT01 automatically received the Company Data (S:) drive after Group Policy was applied, and read/write access was confirmed by creating a test file in the shared folder.

Screenshots

1. Group Policy Management showing the CompanyData Drive Mapping GPO.

<img width="1918" height="1041" alt="05 lab #1" src="https://github.com/user-attachments/assets/ed92e753-3ca6-4ff4-9c56-d75fe5eb3c62" />

2. Drive Mapping GPO configured for \\DC01\CompanyData.

<img width="1918" height="1041" alt="05 lab #2" src="https://github.com/user-attachments/assets/e7e9283b-41d4-4359-9685-d6ae64248b36" />

3. Company Data (S:) drive visible on CLIENT01.

<img width="1920" height="1041" alt="05 lab #3" src="https://github.com/user-attachments/assets/6d007c4a-b126-4336-9ef3-79ecadfebf06" />

4. Test file successfully created inside the mapped drive.

<img width="1893" height="1041" alt="05 lab #4" src="https://github.com/user-attachments/assets/2c8dd143-7d33-4133-a62d-35a2c51db489" />


## Skills Demonstrated

- Active Directory Group Policy Management
- Group Policy Preferences
- Network drive mapping
- SMB file sharing
- Windows client/domain administration
- GPO troubleshooting and verification
- User access and file permissions

## Key Takeaway

This lab demonstrated how Group Policy Preferences can be used to centrally configure resources for domain users. Drive mapping through GPO provides a scalable way for administrators to give users consistent access to shared company resources without manually configuring each workstation.
