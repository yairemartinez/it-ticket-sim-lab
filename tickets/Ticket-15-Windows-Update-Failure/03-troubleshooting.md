# Troubleshooting – Windows Update Failure

## Initial Symptoms
- Windows Update failed or stalled when checking for updates.
- No indication of network connectivity issues or system instability.

<img width="600" height="400" alt="Screenshot 2026-01-29 160907" src="https://github.com/user-attachments/assets/bfa6d25d-37b0-4a09-965c-1a1d0bff9998" />

---

## Step 1: Review Update Services
- Opened Services on WIN11-02.
- Reviewed the status of required update-related services:
  - Windows Update
  - Background Intelligent Transfer Service (BITS)

Observed inconsistent or stopped service behavior during update attempts.

<img width="600" height="400" alt="Screenshot 2026-01-29 153148" src="https://github.com/user-attachments/assets/1ed007e1-b284-498f-979d-606c8c7a9243" />

<img width="600" height="400" alt="Screenshot 2026-01-29 153222" src="https://github.com/user-attachments/assets/0f140d7b-97d9-426b-bb3b-2227a72689b7" />

---

## Step 2: Review System Logs
- Opened Event Viewer.
- Navigated to:
  Windows Logs → System
- Reviewed update-related warnings and errors logged during update attempts.

This confirmed the issue was service-related rather than a system or network failure.

---

## Conclusion
Windows Update failed due to update-related services not operating correctly, preventing update checks from completing.
