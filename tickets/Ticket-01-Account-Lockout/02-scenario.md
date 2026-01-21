# Scenario – User Account Locked

## Environment
- Domain: lab.local
- Domain Controller: SRV-CORE01 (Windows Server 2022)
- Client Workstation: WIN11-01 (Windows 11 Pro)
- Network: Static IP addressing

## Scenario Description
A domain user account was intentionally locked by repeatedly attempting to log in with an incorrect password from a domain-joined Windows 11 workstation.

This scenario simulates a common real-world help desk issue where a user becomes locked out due to repeated failed authentication attempts, often caused by an incorrect or outdated password.

## User Involved
- Username: andy smith
- Domain: lab.local

## Trigger Method
- Multiple failed login attempts were made on WIN11-01 using an incorrect password.
- The domain account lockout policy was reached, resulting in the account being locked.

