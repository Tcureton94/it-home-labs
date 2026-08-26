Objective
Create and deploy a Group Policy Object (GPO) to restrict user access to the Control Panel and PC Settings.

Environment
Windows Server 2022 (DC01)
Windows 11 Enterprise Client
Active Directory domain: homelab.local
Steps
Opened Group Policy Management on DC01.
Created a Group Policy Object named Disable Control Panel.
Linked the GPO to the homelab.local domain.
Enabled Prohibit access to Control Panel and PC settings.
Ran gpupdate /force on the Windows 11 client.
Verified that the policy prevented access to the Control Panel.
Result
The Group Policy successfully applied to the domain-joined Windows 11 client.

When attempting to open the Control Panel, access was blocked and Windows displayed:

This operation has been canceled due to restrictions in effect on this computer.

This confirmed that the GPO was successfully deployed and enforced.

Screenshots
Group Policy Management Console
Opened the Group Policy Management Console on DC01 and expanded the homelab.local domain.

GPO Created
Created a new Group Policy Object named Disable Control Panel.

GPO Linked to Domain
Linked the GPO to the homelab.local domain so the policy would apply to domain users and computers.

Group Policy Updated
Ran gpupdate /force on the Windows 11 client to immediately apply the updated Group Policy.

Policy Verification
Attempted to open Control Panel and confirmed that access was blocked, verifying that the Group Policy was successfully applied.

Skills Practiced
Active Directory
Group Policy Management
Windows Administration
Group Policy Updates
Troubleshooting
Lessons Learned
Learned how to create and link a Group Policy Object (GPO).
Learned how to deploy user policies through Active Directory.
Used gpupdate /force to apply policy changes immediately.
Verified policy deployment by testing on a domain-joined Windows 11 client.
