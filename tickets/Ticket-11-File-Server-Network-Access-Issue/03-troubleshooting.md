# Troubleshooting – File Server Access Failure

## Initial Symptoms
- Hostname-based access to the file server failed
- IP-based access remained functional
- Network drives intermittently disappeared from File Explorer

<img width="600" height="400" alt="Screenshot 2026-01-28 135643" src="https://github.com/user-attachments/assets/ac3c3f19-1b38-432b-b2c5-4b05bf2c2c10" />

---

## Step 1: Test Network Connectivity
Connectivity to the file server was tested using the IP address.

Command used:
ping 10.0.0.10

Result:
- Ping successful, confirming network connectivity was intact

---

## Step 2: Test Name Resolution
Hostname-based connectivity tests failed.

Commands used:
ping SRV-CORE01  
\\SRV-CORE01\DeptShare

Result:
- Hostname resolution failed
- UNC path using hostname was inaccessible


---

## Step 3: Verify IP-Based UNC Access
The same file share was accessed using the IP address.

UNC path tested:
\\10.0.0.10\DeptShare

Result:
- File share opened successfully

<img width="600" height="400" alt="Screenshot 2026-01-28 140347" src="https://github.com/user-attachments/assets/37114261-fa19-44f2-b962-f17448f8ba15" />

---

## Step 4: Review Client DNS Configuration
Client DNS settings were reviewed.

Command used:
ipconfig /all

Finding:
- DNS server was set to a non-existent address (10.0.0.99)

---

## Step 5: Observe Network Drive Behavior
When DNS was misconfigured:
- Network locations disappeared from File Explorer

<img width="600" height="400" alt="Screenshot 2026-01-28 135757" src="https://github.com/user-attachments/assets/703b29e9-f06c-4bd1-88c2-222a10c84f04" />

After reboot and DNS correction:
- Network locations reappeared automatically

<img width="600" height="400" alt="Screenshot 2026-01-28 140818" src="https://github.com/user-attachments/assets/34483059-50c4-432e-8851-2a2c4bd7dcbb" />

---

## Conclusion
The issue was isolated to client-side DNS misconfiguration, not permissions or SMB services.
