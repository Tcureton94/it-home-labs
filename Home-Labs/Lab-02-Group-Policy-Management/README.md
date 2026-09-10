# Lab 02 - Group Policy Management

## Objective

Create and deploy a Group Policy Object (GPO) to restrict user access to the Control Panel and PC Settings.

## Environment

- Windows Server 2022 (DC01)
- Windows 11 Enterprise Client
- Active Directory Domain: `homelab.local`

## Steps

1. Opened Group Policy Management on DC01.
2. Created a Group Policy Object named **Disable Control Panel**.
3. Linked the GPO to the `homelab.local` domain.
4. Enabled **Prohibit access to Control Panel and PC settings**.
5. Ran `gpupdate /force` on the Windows 11 client.
6. Verified that the policy prevented access to Control Panel.

## Result

The Group Policy was successfully applied to the domain-joined Windows 11 client.

When attempting to open Control Panel, Windows displayed:

> This operation has been canceled due to restrictions in effect on this computer.

This confirmed that the GPO was successfully deployed and enforced.

## Screenshots

### Group Policy Management Console

Opened the Group Policy Management Console on DC01 and expanded the `homelab.local` domain.

<img width="1920" height="1080" alt="lab 02 #1" src="https://github.com/user-attachments/assets/229185a2-a3a6-4166-a8d4-08b5d166d202" />

### GPO Created

Created a new Group Policy Object named **Disable Control Panel**.

<img width="1920" height="1080" alt="02 lab #2" src="https://github.com/user-attachments/assets/0e89d5e3-459f-4bf3-9e52-e930eedb64f7" />

### GPO Linked to Domain

Linked the GPO to the `homelab.local` domain so the policy could be applied to domain-joined computers and users.

<img width="1920" height="1080" alt="02 lab #3" src="https://github.com/user-attachments/assets/4da1ef67-e840-4c99-b69a-d36f9ec72098" />

### Group Policy Updated

Ran `gpupdate /force` on the Windows 11 client to immediately apply the updated Group Policy.

<img width="1920" height="1080" alt="lab 02 #4" src="https://github.com/user-attachments/assets/109538d4-f537-4789-ad69-288103743a99" />

### Policy Verification

Attempted to open Control Panel and confirmed that access was blocked, verifying that the Group Policy was successfully applied.

<img width="1920" height="1080" alt="lab 02 #5" src="https://github.com/user-attachments/assets/0f95d9eb-8d61-433c-a2c3-2603759a7a80" />

## Skills Practiced

- Active Directory
- Group Policy Management
- Windows Administration
- Group Policy Updates
- Troubleshooting

## Lessons Learned

- Learned how to create and link a Group Policy Object (GPO).
- Learned how to deploy user policies through Active Directory.
- Used `gpupdate /force` to apply policy changes immediately.
- Verified policy deployment by testing on a domain-joined Windows 11 client.
