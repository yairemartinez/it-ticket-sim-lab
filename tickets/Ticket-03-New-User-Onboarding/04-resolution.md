# Resolution – New User Provisioning

## Resolution Steps
1. Created a new domain user account for ben jones in Active Directory.
2. Assigned the user to the appropriate Help Desk security group.
3. Created a dedicated home directory with correct NTFS permissions.
4. Configured the home directory mapping in the user account settings.

### Step 1: Create Domain User Account

A new domain user account was created in Active Directory for the incoming employee.

<img width="600" height="400" alt="Screenshot 2026-01-21 124659" src="https://github.com/user-attachments/assets/039bc81a-302e-4044-9800-ffe671774517" />

The account was configured with a temporary password and forced password change at next logon.

<img width="600" height="400" alt="Screenshot 2026-01-21 124824" src="https://github.com/user-attachments/assets/8823e531-ea60-4f5e-865b-2c35a878b4e9" />

### Step 2: Assign Group-Based Access

The user was added to the appropriate security group to ensure role-based access control.

<img width="600" height="400" alt="Screenshot 2026-01-21 125402" src="https://github.com/user-attachments/assets/e455e41f-147f-4469-8dc3-0fdb8e42c431" />

### Step 3: Create and Secure Home Directory

A dedicated home directory was created for the user with least-privilege permissions.

- User granted Modify access
- Administrators retained Full Control

<img width="600" height="400" alt="Screenshot 2026-01-21 133637" src="https://github.com/user-attachments/assets/422dd80e-1413-4026-b58b-f37b13219c54" />

The home directory was mapped to drive H: via the user account properties.

<img width="600" height="400" alt="Screenshot 2026-01-21 134707" src="https://github.com/user-attachments/assets/9de5af06-7686-4496-a95d-358bce027a3f" />

## Validation

The user successfully logged in to the domain workstation and accessed assigned resources.

- Login completed successfully
- Home drive (H:) was automatically mapped and accessible

<img width="600" height="400" alt="Screenshot 2026-01-21 135232" src="https://github.com/user-attachments/assets/46a8c049-f68d-4fc6-95b2-cec79fdca080" />

---


