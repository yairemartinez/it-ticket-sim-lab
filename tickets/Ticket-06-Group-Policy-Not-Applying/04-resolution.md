# Resolution – Correcting GPO Scope

## Resolution Steps
- Reviewed the existing Group Policy Object configuration.
- Identified that the GPO contained user configuration settings but was linked to a computer OU.
- Removed the GPO link from the `LAB\Workstations` OU.
- Linked the GPO to the correct `LAB\Users` OU.
- Forced a Group Policy update on the client system.

<img width="800" height="400" alt="Screenshot 2026-01-26 112236" src="https://github.com/user-attachments/assets/70acdbeb-261d-4984-a4dd-d96835a5a52a" />

---

## Validation
- Forced a Group Policy refresh and re-logged the user.
- Confirmed the policy was applied under User Configuration.
- Verified the user was blocked from accessing Control Panel and PC settings.

<img width="800" height="400" alt="Screenshot 2026-01-26 111655" src="https://github.com/user-attachments/assets/3031ba05-4ba5-479c-8d57-758084c5f33f" />



<img width="800" height="400" alt="Screenshot 2026-01-26 111842" src="https://github.com/user-attachments/assets/56a0c2a7-6084-4996-9a53-ee80732729b4" />

---

## Outcome
The Group Policy Object applied successfully once it was linked to the appropriate user OU, and the access restriction was enforced as intended.
