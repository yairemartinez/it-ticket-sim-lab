# Scenario – Authentication Failure Due to Time Sync Issue

## Environment
- **Domain:** lab.local
- **Domain Controller:** SRV-CORE01
- **Client Workstation:** WIN11-02 (Windows 11 Pro)

## Scenario Description
A domain user reported authentication failures when attempting to access domain resources despite using correct credentials.

This scenario simulates a common authentication issue caused by system time drift on a domain-joined client.

## Lab Simulation
Time synchronization on the client workstation was disrupted, resulting in a mismatch between the client system time and the domain controller.

## Observed Behavior
- Authentication failures occurred.
- Client system time differed from domain controller time.
