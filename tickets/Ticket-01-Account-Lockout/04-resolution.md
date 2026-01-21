# 04-resolution.md — Fix & Validation

This must be **clear and repeatable**.

# Resolution – Unlocking Account and Restoring Access

## Resolution Steps
1. Opened Active Directory Users and Computers on SRV-CORE01.
2. Navigated to LAB → Users → andy smith.
3. Unchecked the “Account is locked out” option.
4. Applied the change to unlock the account.

Alternatively, the account was unlocked using PowerShell:

```powershell
Unlock-ADAccount -Identity johndoe
