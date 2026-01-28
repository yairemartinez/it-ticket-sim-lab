# Troubleshooting – DNS Resolution Failure

## Initial Symptoms
- Client unable to resolve internal hostnames
- Network connectivity appeared normal

---

## Step 1: Verify Client DNS Configuration
Reviewed the client network configuration using `ipconfig /all`.

Confirmed the DNS server was configured to a public DNS address (8.8.8.8) instead of the internal DNS server.

<img width="600" height="400" alt="Screenshot 2026-01-27 155710" src="https://github.com/user-attachments/assets/04287e13-192b-4669-b7bf-d8a7c1ebc038" />

---

## Step 2: Test DNS Resolution Using nslookup
Tested name resolution against a public DNS server.

Command used:
nslookup SRV-CORE01 8.8.8.8

The query failed, confirming the public DNS server could not resolve internal hostnames.

<img width="800" height="400" alt="Screenshot 2026-01-27 215713" src="https://github.com/user-attachments/assets/4f29148b-844a-4e24-bc66-b0201c6a42d6" />

---

## Step 3: Verify Network Connectivity by IP
Tested connectivity directly to the domain controller by IP address.

Command used:
ping 10.0.0.10

The ping succeeded, confirming the issue was not related to network connectivity.


---

## Step 4: Confirm Internal DNS Functionality
Tested name resolution directly against the internal DNS server.

Command used:
nslookup SRV-CORE01 10.0.0.10

The hostname resolved successfully.

<img width="800" height="400" alt="Screenshot 2026-01-27 220353" src="https://github.com/user-attachments/assets/84e794e0-8d6b-433f-ad49-f92416e171db" />

---

## Conclusion
The issue was isolated to DNS resolution caused by incorrect client-side DNS configuration.
