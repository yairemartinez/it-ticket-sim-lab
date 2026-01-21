# Prevention – Preventing Permission Issues

## Prevention Steps
- Used group-based permissions instead of assigning access directly to users.
- Ensured share permissions were configured to support the intended level of NTFS access.
- Reviewed both share and NTFS permissions during access provisioning.

## Operational Notes
- Effective access is determined by the most restrictive permission between share and NTFS layers.
- Share permissions should not be more restrictive than the intended NTFS permissions.
- NTFS permissions should be used as the primary mechanism for enforcing least-privilege access.

## Escalation Criteria
- Access issues affecting multiple users or groups.
- Inconsistent access behavior after permission changes.
- Unclear or undocumented permission requirements.
