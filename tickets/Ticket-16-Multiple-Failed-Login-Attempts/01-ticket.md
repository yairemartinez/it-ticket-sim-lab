# Ticket-16-Multiple-Failed-Login-Attempts/01-ticket.md

# Ticket 16 – Multiple Failed Login Attempts Detected

**Severity:** Medium  
**Category:** Monitoring / Authentication  
**Environment:** Lab – Windows Server 2022 AD DS  

## Affected User
- **User:** andy smith
- **Workstation:** WIN11-02

## Summary
Multiple failed login attempts were detected for a domain user account, resulting in an account lockout event recorded on the domain controller.

## User Impact
- User was unable to log in due to account lockout.
- Temporary loss of access to workstation resources.

## Initial Symptoms
- Repeated authentication failures.
- Account lockout event logged on the domain controller.

## Triage Summary
- Reviewed domain controller security logs.
- Identified account lockout event and source workstation.
- Determined activity was consistent with user error.

## Root Cause
User entered incorrect credentials multiple times, triggering the account lockout policy.

## Resolution
The account was unlocked after confirming the cause, restoring normal access.

## Validation
User successfully logged in with no further authentication failures.

## Prevention
Authentication monitoring and escalation criteria were documented.

## Time to Resolve
Approximately 10–15 minutes

## Escalation Notes
Escalate if similar authentication failures recur or originate from unknown sources.
