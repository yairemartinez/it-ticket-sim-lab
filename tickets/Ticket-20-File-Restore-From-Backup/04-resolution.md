# Resolution – Restoring Time Synchronization

## Resolution Steps
1. Identified time drift on the client workstation.
2. Restarted the Windows Time service on WIN11-02.
3. Re-enabled domain time synchronization.
4. Forced a time resynchronization with the domain controller.

```cmd
w32tm /resync
