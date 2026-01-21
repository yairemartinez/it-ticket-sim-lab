# Ticket 01 – User Account Locked After Multiple Failed Logins

**Severity:** Medium  
**Category:** Account Access  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Summary
A domain user was unable to log in due to their account being locked after multiple failed authentication attempts.

## User Impact
The user could not sign in to their workstation or access domain resources.

## Initial Symptoms
The user reported repeated login failures followed by an account lockout message.

## Triage Summary
- Verified account lockout status in Active Directory
- Reviewed domain controller security logs
- Identified the workstation responsible for the lockout

## Root Cause
The account was locked due to repeated authentication attempts using an incorrect password from a domain-joined workstation, triggering the domain account lockout policy.

## Resolution
The account was unlocked and access was restored after verifying the source of the lockout.

## Validation
The user successfully logged in after the account was unlocked, and no further lockouts were observed.

## Prevention
Lockout investigation steps were documented, and credential hygiene guidance was noted to prevent recurrence.

## Time to Resolve
Approximately 10–15 minutes factoring in user interaction.

## Escalation Notes
Escalate if lockouts continue or originate from unknown systems.

