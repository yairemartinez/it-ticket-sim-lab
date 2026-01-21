# Troubleshooting – Account Lockout Investigation

## Initial Symptoms
- User was unable to log in and received an account lockout message at the Windows login screen.

## Step 1: Confirm Account Lockout in Active Directory
Active Directory Users and Computers was used to verify the account status.

- Navigated to: LAB → Users → andy smith
- Confirmed the account was marked as locked

<img width="800" height="600" alt="Screenshot 2026-01-20 231858" src="https://github.com/user-attachments/assets/3d8cd7b8-401a-4f92-b6ca-b69332dc6a99" />

---

## Step 2: PowerShell Verification
PowerShell was used on the domain controller to confirm the lockout status.

```powershell
Get-ADUser johndoe -Properties LockedOut | Select Name, LockedOut
