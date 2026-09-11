Lab 04 - Shared Folder & NTFS Permissions
## Objective
Create a shared folder on Windows Server 2022, configure Share and NTFS permissions, and verify that a domain user can access and modify the shared folder from a Windows 11 client.

## Environment
- Windows Server 2022 (DC01)
- Windows 11 Enterprise Client (CLIENT01)
- Active Directory Domain: homelab.local

## What I Did
- Created a shared folder named CompanyData on the C: drive.
- Configured Advanced Sharing for the folder.
- Assigned Share permissions to Domain Users.
- Configured NTFS permissions using the Security tab.
- Granted Domain Users Modify permissions.
- Removed the default Everyone group from Share permissions.
- Accessed the shared folder from CLIENT01 using the UNC path.
- Verified that a domain user could successfully create a file within the shared folder.

## Results
Successfully configured and tested a Windows file share using both Share and NTFS permissions. Verified that a standard domain user (Mike Davis) could access the shared folder and create a test file over the network.

## Screenshots

1. CompanyData Share Permissions configured for Domain Users.

<img width="1916" height="1037" alt="04 lab #1" src="https://github.com/user-attachments/assets/f20ef3c9-5417-4e3e-899b-beb4b37e0bca" />

2. Domain Users configured with Modify NTFS permissions.

<img width="1904" height="1041" alt="04 lab #2" src="https://github.com/user-attachments/assets/79dd461a-1ba4-40f4-9f57-510fdd889c7d" />

3. CLIENT01 successfully accessing \\DC01\CompanyData and creating Lab04-Test.txt.

<img width="1890" height="1041" alt="04 lab #3" src="https://github.com/user-attachments/assets/22d631a5-02a6-4bd0-98dc-a543be36479d" />


## What I Learned
This lab helped me understand the difference between Share permissions and NTFS permissions. I learned that Share permissions control network access, while NTFS permissions control access to files and folders stored on the disk. I also verified that a standard domain user could access a shared folder using the appropriate permissions, reinforcing how Windows manages file sharing in an Active Directory environment.
