# Ticket 06 – Group Policy Not Applying to User

**Severity:** Medium  
**Category:** Group Policy  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Summary
A Group Policy Object did not apply as expected to a domain user.

## User Impact
The user retained access to restricted system settings.

## Initial Symptoms
Configured policy did not take effect after user login.

## Triage Summary
- Reviewed applied group policies
- Checked GPO scope and OU linkage

## Root Cause
The GPO was linked to a computer OU while containing user configuration settings.

## Resolution
The GPO was linked to the correct user OU and applied successfully.

## Validation
The policy applied correctly and restricted access as intended.

## Prevention
Proper GPO scoping practices were documented.

## Time to Resolve
Approximately 30–40 minutes

## Escalation Notes
Escalate if policies fail across multiple OUs or inheritance conflicts are identified.

