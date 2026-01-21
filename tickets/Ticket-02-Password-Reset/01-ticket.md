# Ticket 02 – Password Reset With Forced Change at Next Logon

**Severity:** Low  
**Category:** Account Access  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Summary
A domain user requested assistance after forgetting their password and being unable to log in.

## User Impact
The user could not access their workstation or domain resources.

## Initial Symptoms
The user reported login failures due to an unknown or forgotten password.

## Triage Summary
- Verified user identity
- Confirmed account was active and not locked

## Root Cause
The user was unable to authenticate due to a forgotten password.

## Resolution
The account password was reset, and the user was required to change the password at next logon.

## Validation
The user successfully logged in and completed a password change.

## Prevention
Password reset best practices were followed to reduce security risk.

## Time to Resolve
Approximately 5–10 minutes

## Escalation Notes
Escalate if repeated reset requests occur or account misuse is suspected.

