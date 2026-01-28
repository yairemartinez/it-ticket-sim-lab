# Resolution – Restoring File Server Access

## Resolution Steps
1. Updated the client DNS configuration to use the internal domain DNS server (10.0.0.10).
2. Flushed the DNS resolver cache.
3. Restarted the client to ensure network resources refreshed correctly.

Command used:
ipconfig /flushdns

<img width="600" height="400" alt="Screenshot 2026-01-28 140102" src="https://github.com/user-attachments/assets/4bcf5500-2215-432a-b993-d313d7cc59b1" />

---

## Validation
- Access to `\\SRV-CORE01\DeptShare` succeeded
- Network drives consistently reappeared in File Explorer
- No credential prompts occurred after correction

<img width="600" height="400" alt="Screenshot 2026-01-28 140255" src="https://github.com/user-attachments/assets/e83528c6-1dc1-4a3e-a8df-1d8708c71343" />
