# Troubleshooting – Network Drive Mapping Failure

## Initial Symptoms
- User logged in successfully but the expected Z: network drive did not appear.
- The shared folder was accessible manually via UNC path, but not mapped.

<img width="800" height="400" alt="Screenshot 2026-01-26 220345" src="https://github.com/user-attachments/assets/9816adda-2da5-422e-a8c5-f1ea8cbee54f" />

---

## Step 1: Verify GPO Application
- Ran `gpresult /r` to identify applied user policies.
- Confirmed the drive mapping GPO was not initially listed under User Settings.

<img width="800" height="400" alt="Screenshot 2026-01-26 220833" src="https://github.com/user-attachments/assets/2ea36add-d253-4b9f-89ab-50543f5d2f7a" />

---

## Step 2: Verify Share and NTFS Permissions
- Confirmed the shared folder existed and was accessible.
- Verified NTFS permissions granted Modify access to the appropriate security group.
- Verified the folder was shared correctly on the file server.

<img width="800" height="400" alt="Screenshot 2026-01-26 211618" src="https://github.com/user-attachments/assets/022e015b-7cfa-4768-bd59-7229ac01a28f" />



<img width="800" height="400" alt="Screenshot 2026-01-26 214126" src="https://github.com/user-attachments/assets/9c3b4d3f-83a3-4e50-affa-7d39484e97b6" />

---

## Step 3: Review GPO Configuration
- Verified the drive mapping was configured under User Configuration → Preferences.
- Confirmed the GPO was linked to the correct Users OU.

<img width="800" height="400" alt="Screenshot 2026-01-26 212445" src="https://github.com/user-attachments/assets/0c14b70d-44cb-42df-8fcf-7a40f2722a1a" />



<img width="800" height="400" alt="Screenshot 2026-01-26 214818" src="https://github.com/user-attachments/assets/e1ef56a0-64f3-4e3f-a545-4264e86527c2" />

---

## Step 4: Identify Security Filtering Issue
- Determined the drive mapping GPO only applied when Authenticated Users were present.
- Removing Authenticated Users prevented Group Policy Preferences from executing.
- Confirmed this behavior by re-adding Authenticated Users and retesting.

---

## Lessons Learned
- Group Policy Preferences may fail silently if Authenticated Users is removed from security filtering.
- Drive mapping GPOs should retain Authenticated Users and use item-level targeting for restriction.
- `gpresult` and RSOP are essential tools for verifying GPO and preference processing.
