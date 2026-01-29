# Troubleshooting – Disk Space Alert

## Initial Symptoms
- User reported low disk space warnings.
- C: drive showed critically low free space.

---

## Step 1: Verify Disk Usage
- Opened File Explorer on WIN11-01.
- Navigated to **This PC**.
- Confirmed the system drive (C:) was nearly full and displayed as low disk space.

<img width="600" height="400" alt="Screenshot 2026-01-29 135403" src="https://github.com/user-attachments/assets/e8bb3b31-dcab-42ea-b6f9-256a58220c1c" />
<img width="600" height="400" alt="Screenshot 2026-01-29 135927" src="https://github.com/user-attachments/assets/81f4c029-c12f-43ae-8279-6f4ae43b3903" />

---

## Step 2: Identify Disk Usage Sources
- Opened **Settings → System → Storage**.
- Reviewed storage usage by category.
- Identified unusually large files located within the user profile, specifically on the Desktop.

<img width="600" height="400" alt="Screenshot 2026-01-29 135714" src="https://github.com/user-attachments/assets/00ab6b8b-5ee7-4dfc-81f1-6e2912637eb8" />
<img width="600" height="400" alt="Screenshot 2026-01-29 135725" src="https://github.com/user-attachments/assets/0ef03514-1772-406c-96d2-e9da6d9df486" />

---

## Conclusion
The low disk space condition was caused by large user-level files consuming available storage on the system drive.
