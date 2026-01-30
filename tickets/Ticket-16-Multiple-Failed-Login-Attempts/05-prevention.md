# Prevention – Monitoring Authentication Failures

## Prevention Steps
- Documented steps for reviewing authentication-related security logs.
- Reinforced correct credential usage with the user.
- Monitored for additional failed login attempts after resolution.

## Operational Notes
- Event ID 4740 provides authoritative confirmation of account lockouts.
- Failed login attempts may also generate Event ID 4625, which can be distributed across systems.
- Repeated failures from a single workstation often indicate user error, while distributed sources may indicate risk.

## Escalation Criteria
Escalate to systems administration or security teams if:
- Failed logins originate from multiple workstations.
- Lockouts occur repeatedly for the same account.
- Authentication failures involve unknown or unexpected source systems.
