# Troubleshooting – Temporary Profile Issue

## Initial Symptoms
- User logged in and received a warning stating Windows could not sign in to the account.
- User was logged in with a temporary profile.
- Desktop appeared reset to default.
- User files and personalized settings were unavailable.

<img width="600" height="400" alt="Screenshot 2026-01-29 120720" src="https://github.com/user-attachments/assets/343b990a-29bb-4fd7-810a-5f06dd306d15" />


<img width="600" height="400" alt="Screenshot 2026-01-29 120736" src="https://github.com/user-attachments/assets/eacd5ebf-9ae6-4e61-9147-104b8da72438" />

---

## Step 1: Review Event Logs
- Opened Event Viewer on WIN11-01.
- Navigated to:
  Windows Logs → Application
- Identified User Profile Service errors occurring at the time of user login.

### Relevant Events
- **Event ID 1511** – Windows could not find the local user profile.
- **Event ID 1515** – Windows logged the user on with a temporary profile.

These events indicate Windows failed to load the assigned user profile and generated a temporary profile for the session.

<img width="800" height="400" alt="Screenshot 2026-01-29 121331" src="https://github.com/user-attachments/assets/318832ea-9e78-492e-bd85-17ca8c8c5982" />

---

## Step 2: Review User Profile Directory
- Navigated to `C:\Users`.
- Confirmed the expected profile folder `benjones` was not present.
- Verified the original profile directory had been renamed to `benjones.old`.

This prevented Windows from locating the correct profile path during login.

<img width="600" height="400" alt="Screenshot 2026-01-29 120533" src="https://github.com/user-attachments/assets/fda97b6e-b17f-43f3-9333-dc97e592da8f" />

---

## Conclusion
Windows was unable to load the user profile due to an inaccessible profile directory, resulting in the assignment of a temporary profile during login.
