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

![Group Policy Management Console](images/lab%2002%201.png)

### GPO Created

Created a new Group Policy Object named **Disable Control Panel**.

![GPO Created](images/02%20lab%202.png)

### GPO Linked to Domain

Linked the GPO to the `homelab.local` domain so the policy could be applied to domain-joined computers and users.

![GPO Linked to Domain](images/02%20lab%203.png)

### Group Policy Updated

Ran `gpupdate /force` on the Windows 11 client to immediately apply the updated Group Policy.

![Group Policy Updated](images/lab%2002%204.png)

### Policy Verification

Attempted to open Control Panel and confirmed that access was blocked, verifying that the Group Policy was successfully applied.

![Policy Verification](images/lab%2002%205.png)

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
