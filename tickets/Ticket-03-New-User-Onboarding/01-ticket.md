# Ticket 03 – New User Onboarding (Account, Groups, Home Directory)

**Severity:** Low  
**Category:** Account Management  
**Environment:** Lab – Windows Server 2022 AD DS, Windows 11 Pro Client  

## Summary
A new employee required onboarding into the Active Directory environment.

## User Impact
The user could not begin work without a domain account and access.

## Initial Request
Request received to provision a new domain user account with standard Help Desk access.

## Triage Summary
- Verified user did not already exist
- Identified correct OU and security groups

## Root Cause
New user account had not yet been created.

## Resolution
A new domain user account was created, assigned to appropriate groups, and provisioned with a home directory.

## Validation
The user successfully logged in and accessed assigned resources.

## Prevention
Standard onboarding practices were followed to ensure consistency.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate if access requirements are unclear or additional permissions are requested.
