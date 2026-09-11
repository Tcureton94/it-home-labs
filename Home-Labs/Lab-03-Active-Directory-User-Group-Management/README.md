## Lab 03 - Active Directory User & Group Management

# Objective

Create Organizational Units (OUs), user accounts, and security groups, then assign users to the appropriate groups.

## Environment

- Windows Server 2022 (DC01)
- Active Directory Users and Computers (ADUC)
- Active Directory domain: `homelab.local`

## Steps

1. Created Organizational Units (OUs) to organize Active Directory objects.
2. Created five domain user accounts:
   - Emily Brown
   - Mike Davis
   - Sarah Johnson
   - John Smith
   - David Wilson
3. Created four security groups:
   - Sales Team
   - IT Support
   - HR Team
   - Employees
4. Assigned users to their appropriate security groups.
5. Verified that users were assigned to the correct security groups.

## Result

Successfully created and organized users, Organizational Units, and security groups in Active Directory.

Verified that users were assigned to the appropriate security groups.

## Screenshots

### Organizational Units and Groups

Created and organized Organizational Units and security groups within the `homelab.local` Active Directory domain.

<img width="1917" height="1041" alt="lab 03 #1" src="https://github.com/user-attachments/assets/27b4fe57-a1cf-4f2b-9685-8258a248b3ab" />

### IT Support Group Membership

Verified that Mike Davis was assigned to the **IT Support** security group.

<img width="1920" height="1041" alt="lab 03 #2" src="https://github.com/user-attachments/assets/3f851dd1-0f3c-4775-a722-66b9e1d10cf6" />

## Lessons Learned

- Learned how Organizational Units (OUs) are used to organize Active Directory objects.
- Learned how to create and manage domain user accounts.
- Learned how to create security groups and assign users to them.
- Practiced using group membership to organize users and manage access within a Windows domain environment.
