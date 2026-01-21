# Troubleshooting – Shared Folder Access Issue

## Initial Symptoms
- User received an “Access Denied” message when attempting to access the shared folder.

<img width="800" height="400" alt="Screenshot 2026-01-21 154800" src="https://github.com/user-attachments/assets/6ffab251-70b8-4604-990c-7e22d13f77fb" />

---

## Step 1: Confirm Network Connectivity
- Verified the file server was reachable via hostname.
- Confirmed no network connectivity issues.

---

## Step 2: Review Share Permissions
- Reviewed the share permissions on \\SRV-CORE01\DeptShare.
- Confirmed share permissions allowed read access.

![Share permissions](./screenshots/share-permissions.png)

---

## Step 3: Review NTFS Permissions
- Reviewed NTFS permissions on C:\Shares\DeptShare.
- Identified that the user’s security group was missing.

<img width="800" height="400" alt="Screenshot 2026-01-21 155134" src="https://github.com/user-attachments/assets/a7c899d6-d387-460a-92f3-b55fa67b3612" />

---

## Conclusion
The issue was determined to be caused by restrictive NTFS permissions despite permissive share permissions.

