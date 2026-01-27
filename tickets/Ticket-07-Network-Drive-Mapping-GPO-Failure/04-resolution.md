# Resolution – Restoring Network Drive Mapping

## Resolution Steps
1. Forced a Group Policy update on the client.
2. Logged out and logged back in to refresh user policy processing.

```powershell
gpupdate /force
