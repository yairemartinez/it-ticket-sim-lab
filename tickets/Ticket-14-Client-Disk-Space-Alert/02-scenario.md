# Scenario – Client Disk Space Alert

## Environment
- **Client Workstation:** WIN11-01 (Windows 11 Pro)
- **Domain User:** ben jones

## Scenario Description
A domain user received a low disk space alert indicating that the system drive (C:) was critically low on available storage.

This scenario simulates a common endpoint maintenance issue requiring verification and safe cleanup without impacting system stability or user data.

## Lab Simulation
To safely reproduce the issue, a large non-essential file was created in the user profile to intentionally consume disk space and trigger Windows alerts.

## Observed Behavior
- C: drive displayed in red in File Explorer.
- Windows generated a low disk space warning.

<img width="600" height="400" alt="Screenshot 2026-01-29 135403" src="https://github.com/user-attachments/assets/b60f752b-6016-49e1-9875-aa1984ed4ab6" />
