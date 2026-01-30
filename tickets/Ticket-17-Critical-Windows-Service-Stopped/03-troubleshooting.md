# Troubleshooting – Service Failure

## Initial Symptoms
- A critical Windows service was found in a stopped state on the server.

<img width="800" height="800" alt="Screenshot 2026-01-30 143800" src="https://github.com/user-attachments/assets/daba49a4-0ef3-495d-9873-22caca058462" />

---

## Step 1: Review Service Status
- Opened Services on SRV-CORE01.
- Verified the Print Spooler service status was **Stopped**.
- Confirmed the startup type was set to **Automatic**.

---

## Step 2: Review System Logs
- Opened Event Viewer on SRV-CORE01.
- Navigated to:
  Windows Logs → System
- Identified **Service Control Manager** event entries related to the Print Spooler service.

### Relevant Event
- **Event ID 7036** – Service entered the stopped state.

<img width="800" height="800" alt="Screenshot 2026-01-30 144548" src="https://github.com/user-attachments/assets/1b29402a-63c1-4c56-9927-a3bdba4b5828" />

---

## Conclusion
The Print Spooler service stopped in a controlled manner and did not crash or trigger additional system errors.
