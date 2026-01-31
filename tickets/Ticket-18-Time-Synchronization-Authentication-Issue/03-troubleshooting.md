# Troubleshooting – Authentication Failure

## Initial Symptoms
- User reported authentication failures with correct credentials.
- No account lockouts were observed.


---

## Step 1: Verify Account Status
- Confirmed the user account was enabled and not locked.
- Verified no recent password resets or policy changes.

---

## Step 2: Compare System Time
- Checked system time on WIN11-02.
- Checked system time on SRV-CORE01.
- Identified a time difference between the client and domain controller.

<img width="600" height="400" alt="Screenshot 2026-01-30 155422" src="https://github.com/user-attachments/assets/7a5213d1-5c5a-48d6-8133-064979c2ba07" />

---

## Step 3: Review Time Synchronization
- Reviewed Windows Time service status on the client.
- Confirmed time synchronization was not functioning as expected.

<img width="600" height="400" alt="Screenshot 2026-01-30 154940" src="https://github.com/user-attachments/assets/f95f4953-5387-42b5-bc49-00cfe29a60eb" />

---

## Conclusion
Authentication failures were caused by system time drift on the client workstation, exceeding Kerberos authentication tolerance.
