# PHASE 1 — Scenario Setup (Safe, Reversible)

To safely reproduce a temporary profile condition in the lab environment:

1. Logged into WIN11-01 using an administrative account.
2. Navigated to:
   C:\Users
3. Renamed the existing user profile directory:
   benjones → benjones.old

This prevented Windows from locating the expected profile path during login, simulating a corrupted or inaccessible user profile without deleting user data.
