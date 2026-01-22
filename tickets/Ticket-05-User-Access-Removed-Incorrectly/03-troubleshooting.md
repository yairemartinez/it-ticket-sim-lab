# Troubleshooting – Access Restoration Investigation

## Initial Symptoms
- User previously had access to the shared folder.
- User now receives an “Access Denied” error.

<img width="800" height="400" alt="Screenshot 2026-01-21 191023" src="https://github.com/user-attachments/assets/9469896b-d649-4106-b98c-0c062b860bb2" />

---

## Step 1: Confirm Network and Share Availability
- Verified the file server was reachable.
- Confirmed the shared folder was accessible to other authorized users.

---

## Step 2: Review Group Membership
- Checked the user’s group memberships in Active Directory.
- Identified that the user was no longer a member of LAB-HelpDesk.

<img width="800" height="400" alt="Screenshot 2026-01-21 191818" src="https://github.com/user-attachments/assets/a70016ff-02e2-407f-9050-918e88dc6468" />

---

## Step 3: Review Folder Permissions
- Confirmed NTFS permissions grant access to LAB-HelpDesk.
- Verified no direct permissions were assigned to the user.

---

## Conclusion
The access issue was caused by the user being removed from the required security group.

