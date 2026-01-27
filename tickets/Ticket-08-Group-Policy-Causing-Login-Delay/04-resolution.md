# Resolution – Optimizing GPO Scope

## Resolution Steps
1. Reviewed the scope and impact of the user desktop restriction GPO.
2. Reduced the GPO scope by unlinking it from the high-level OU.
3. Linked the GPO only to the appropriate Users OU to limit processing to intended users.
4. Forced a Group Policy update on the client system.

<img width="600" height="1000" alt="Screenshot 2026-01-27 120232" src="https://github.com/user-attachments/assets/f0db6bb3-9776-4ba0-a6f2-39cfccfd8b2f" />

---

```powershell
gpupdate /force
