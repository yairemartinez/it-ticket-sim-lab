# Prevention – Preventing File Server Access Issues

## Prevention Steps
- Ensure all domain-joined clients use internal DNS servers.
- Avoid configuring public or invalid DNS servers on static IP systems.
- Document approved DNS settings for workstation deployments.

## Operational Notes
- DNS issues can mimic permissions or SMB failures.
- Testing access by IP is an effective way to isolate name resolution problems.
- Network drive visibility can fluctuate when name resolution is unstable.

## Escalation Criteria
- Multiple users unable to access file servers
- DNS service outages or misconfigurations affecting multiple systems
