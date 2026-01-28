# Resolution – Correcting DNS Configuration

## Resolution Steps
1. Updated the client DNS configuration to point to the internal DNS server (10.0.0.10).
2. Flushed the DNS resolver cache to remove stale records.

Command used:
ipconfig /flushdns

<img width="800" height="400" alt="Screenshot 2026-01-27 220240" src="https://github.com/user-attachments/assets/cc9ace8a-e210-4079-bb88-49012fb9223f" />

---

## Validation
Verified that internal hostnames could be resolved successfully.

Commands used:
nslookup SRV-CORE01
ping SRV-CORE01

The client successfully resolved and accessed internal resources by hostname.

<img width="800" height="400" alt="Screenshot 2026-01-27 155606" src="https://github.com/user-attachments/assets/02f3e379-69cf-4286-a7b3-9a2eea95f5d6" />
