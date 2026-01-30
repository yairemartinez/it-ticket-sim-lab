# Troubleshooting – Failed Login Pattern

## Initial Symptoms
- User account became locked following repeated login failures.

---

## Step 1: Review Security Logs
- Opened Event Viewer on SRV-CORE01.
- Navigated to:
  Windows Logs → Security
- Identified **Event ID 4740** indicating the user account was locked.

---

## Step 2: Analyze Event Details
- Reviewed Event ID 4740 details.
- Confirmed:
  - Affected user account: andy smith
  - Caller computer name: WIN11-02

This indicated repeated authentication failures originating from a single workstation.

---

## Step 3: Pattern Assessment
- Activity involved a single user and single workstation.
- Logon type was consistent with interactive login attempts.
- No evidence of network-based or distributed authentication attempts.

---

## Conclusion
The authentication failures were consistent with user password entry error rather than malicious activity.
