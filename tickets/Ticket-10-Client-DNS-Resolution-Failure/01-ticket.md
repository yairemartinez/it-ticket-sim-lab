# Ticket 10 – Client Unable to Resolve Internal DNS Names

**Severity:** Medium  
**Category:** Networking / DNS  
**Environment:** Lab – Windows Server 2022 DNS, Windows 11 Pro Client  

## Summary
A domain-joined client was unable to resolve internal hostnames while network connectivity remained functional.

## User Impact
The user could not access internal resources using hostnames, impacting access to domain services.

## Initial Symptoms
- Internal hostnames failed to resolve
- IP-based connectivity remained available

## Triage Summary
- Reviewed client network configuration
- Tested DNS resolution and IP connectivity
- Isolated issue to client-side DNS configuration

## Root Cause
The client was configured to use an external DNS server instead of the internal Active Directory DNS server.

## Resolution
The client DNS configuration was corrected and the DNS cache was flushed.

## Validation
Internal hostnames resolved successfully after DNS correction.

## Prevention
DNS configuration best practices were documented to prevent recurrence.

## Time to Resolve
Approximately 15–20 minutes

## Escalation Notes
Escalate if multiple clients experience DNS resolution failures.
