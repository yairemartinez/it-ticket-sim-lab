# Troubleshooting – Login Failure After Security Policy Change

## Initial Symptoms
- User was unable to log in to the workstation.
- Error message indicated local logon was not permitted.

<img width="800" height="400" alt="Screenshot 2026-01-27 135224" src="https://github.com/user-attachments/assets/0c87c460-e594-4f07-9fe7-fe91d8b894ce" />

---

## Step 1: Identify Recent Changes
- Reviewed recent Group Policy changes affecting workstations.
- Identified a newly created security policy modifying local logon rights.

<img width="800" height="400" alt="Screenshot 2026-01-27 134550" src="https://github.com/user-attachments/assets/1e21fda3-0309-49d3-8955-b260a181e453" />

---

## Step 2: Review GPO Scope and Targeting
- Confirmed the GPO was linked to the **Workstations** OU.
- Verified the policy targeted the **LAB-HelpDesk** security group.

<img width="800" height="400" alt="Screenshot 2026-01-27 134727" src="https://github.com/user-attachments/assets/d784d29c-25b7-44ba-ac32-5578bfd431b0" />

---

## Step 3: Validate Policy Application Method
- Direct gpresult output could not be collected for the affected user due to login denial.
- Administrative accounts were not impacted due to exclusion from the targeted security group.

---

## Conclusion
The login failure was caused by a misconfigured security policy denying local logon rights to the user’s security group.
