# Scenario – Windows Update Failing on Client

## Environment
- **Client Workstation:** WIN11-02 (Windows 11 Pro)
- **Domain User:** ben jones

## Scenario Description
A domain user reported that Windows Updates were failing to complete on their workstation when checking for updates.

This scenario simulates a common endpoint issue where update-related services are not functioning correctly, resulting in update failures without system crashes or network outages.

## Lab Simulation
To safely reproduce the issue, update-related services were stopped, causing Windows Update to fail or hang when checking for updates.

## Observed Behavior
- Windows Update failed or stalled during checks.
- Settings remained accessible after recovery steps were applied.

<img width="600" height="400" alt="Screenshot 2026-01-29 160907" src="https://github.com/user-attachments/assets/d0df329d-a912-45bd-9722-43cc567bc885" />
