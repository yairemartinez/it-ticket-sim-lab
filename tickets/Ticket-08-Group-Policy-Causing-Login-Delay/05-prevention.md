# Prevention – Preventing GPO Performance Issues


## Prevention Steps
- Avoid linking user-scoped policies at high-level OUs unless required.
- Apply new policies with limited scope before broader deployment.
- Review GPO scope as part of performance troubleshooting.


## Operational Notes
- GPO scope is determined by link location and security filtering, not client-side tools.
- Performance considerations should be evaluated alongside functionality.
- Reducing unnecessary policy processing improves scalability and user experience.


## Escalation Criteria
- Login delays affecting multiple users
- Unclear GPO ownership or scope
- Performance issues following policy changes
