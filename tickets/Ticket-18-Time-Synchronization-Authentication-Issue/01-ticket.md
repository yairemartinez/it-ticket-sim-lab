# Ticket 18 – Authentication Failures Due to Time Sync Issue

**Severity:** Medium  
**Category:** Authentication / Time Synchronization  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Affected User
- **User:** andy smith
- **Workstation:** WIN11-02

## Summary
A domain user was unable to authenticate to domain resources due to a system time synchronization issue on the client workstation.

## User Impact
- User authentication attempts failed despite correct credentials.
- Access to domain resources was disrupted.

## Initial Symptoms
- Login and authentication failures reported.
- No account lockouts or password changes occurred.

## Triage Summary
- Verified account status and credentials.
- Investigated system time configuration and synchronization.
- Identified time drift on the client system.

## Root Cause
System time on the client workstation was out of sync with the domain controller, exceeding Kerberos authentication tolerance.

## Resolution
Time synchronization was restored on the client system, resolving the authentication failures.

## Validation
User authentication succeeded after system time was corrected.

## Prevention
Time synchronization best practices were documented.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate if time synchronization issues affect multiple domain systems.
