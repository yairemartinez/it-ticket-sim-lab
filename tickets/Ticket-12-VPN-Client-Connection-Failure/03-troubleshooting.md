# Troubleshooting – VPN Client Connection Failure

## Initial Symptoms
- User could not activate VPN tunnel
- VPN interface not visible to the user

<img width="600" height="400" alt="Screenshot 2026-01-28 231458" src="https://github.com/user-attachments/assets/e1fe68ce-5f92-4a40-89ad-4ad8340f2313" />

---

## Step 1: Verify VPN Service Status
- Confirmed WireGuard service was installed and running.
- Verified no system-wide network outage.

---

## Step 2: Test Under Administrator Account
- Logged in with an administrator account.
- Confirmed VPN tunnel existed and could be activated successfully.

<img width="600" height="400" alt="Screenshot 2026-01-28 231301" src="https://github.com/user-attachments/assets/a9316a99-e6e8-49e1-b70c-86a5be40a0c3" />

---

## Step 3: Test Under Standard User Account
- Logged in as andy smith.
- WireGuard UI could not be accessed.
- Error message indicated UI access restricted to Builtin Administrators.

<img width="600" height="400" alt="Screenshot 2026-01-28 231220" src="https://github.com/user-attachments/assets/e5e4d41d-ad20-4ac0-b545-8e51ff988b1a" />

---

## Conclusion
The issue was caused by user permission limitations, not VPN configuration or connectivity problems.
