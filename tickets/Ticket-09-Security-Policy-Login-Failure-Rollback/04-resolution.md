# Resolution – Rolling Back Security Policy

## Resolution Steps
1. Identified the misconfigured User Rights Assignment.
2. Removed the affected security group from the **Deny log on locally** policy.
3. Updated Group Policy on the affected workstation.

<img width="800" height="400" alt="Screenshot 2026-01-27 143128" src="https://github.com/user-attachments/assets/2ffdc990-160e-463d-9afe-0a29ac89ed9b" />

---

```powershell
gpupdate /force
