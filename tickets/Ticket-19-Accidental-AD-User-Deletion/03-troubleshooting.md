# Troubleshooting – User Account Deletion

## Initial Symptoms
- User unable to authenticate.
- User object missing from Active Directory.

## Login Behavior Observed
- When attempting to log in using the affected user account, the system returned a generic “password is incorrect” message.  
- Given that the credentials were known to be correct and the account was recently functional, this behavior indicated a possible account state issue rather than an actual password error.

## Account Verification

- Checked Active Directory Users and Computers and confirmed the user object was missing.
- Reviewed Active Directory Administrative Center and located the user under Deleted Objects.

---

## Step 1: Verify Deletion
- Confirmed user object was deleted.
<img width="600" height="400" alt="Screenshot 2026-01-30 233725" src="https://github.com/user-attachments/assets/2d229bbd-745a-4bf9-84b5-fa27c7722bb8" />

---

## Step 2: Review Deleted Objects
- Located deleted user object in Active Directory Recycle Bin.
<img width="600" height="400" alt="Screenshot 2026-01-30 233919" src="https://github.com/user-attachments/assets/43f24acb-a1cd-44d2-999f-00fbfcf56c9a" />

---

## Conclusion
The user account was accidentally deleted and recoverable.

