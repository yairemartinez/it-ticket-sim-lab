# Prevention – Reliable Network Drive Mapping


## Prevention Steps
- Retain Authenticated Users in security filtering for GPOs using Group Policy Preferences.
- Use item-level targeting to control which users receive drive mappings.
- Verify GPO application using gpresult and RSOP after changes.


## Operational Notes
- Group Policy Preferences may fail without visible errors if Apply Group Policy permissions are misconfigured.
- UNC paths must be reachable and shared before configuring drive mappings.
- User logoff/logon may be required for drive mappings to appear.


## Escalation Criteria
- Drive mappings failing for multiple users
- GPOs not appearing under User Settings
- Preference settings missing in RSOP
