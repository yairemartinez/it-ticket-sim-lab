# Prevention – Preventing Time Sync Issues

## Prevention Steps
- Ensure domain-joined systems synchronize time with the domain controller.
- Avoid manual time configuration on managed systems.
- Monitor Windows Time service health.

## Operational Notes
- Kerberos authentication is sensitive to time drift.
- Time-related issues can present as credential failures.
- Domain controllers act as the authoritative time source.

## Escalation Criteria
- Time drift affecting multiple systems
- Windows Time service failures on domain controllers
- Widespread authentication issues
