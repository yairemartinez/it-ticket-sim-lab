# Ticket 12 – VPN Client Unable to Connect

**Severity:** Medium  
**Category:** VPN / Remote Access  
**Environment:** Lab – Windows 11 Pro Client, WireGuard VPN  

## Summary
A user reported being unable to activate a VPN connection using the WireGuard client.

## User Impact
The user could not access VPN-protected resources.

## Initial Symptoms
- VPN tunnel not visible to the user
- VPN could not be activated by the user

## Triage Summary
- Verified WireGuard service was running
- Confirmed VPN tunnel existed and functioned under an administrator account
- Identified user permission limitations

## Root Cause
WireGuard tunnel management is restricted to Builtin Administrators.  
The affected user did not have permission to access or manage the VPN client UI.

## Resolution
Issue was escalated to administrators for VPN activation and management.

## Validation
VPN tunnel was confirmed functional when managed by an administrator.

## Prevention
Documented VPN client permission requirements and escalation procedures.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate VPN access requests requiring administrative privileges.
