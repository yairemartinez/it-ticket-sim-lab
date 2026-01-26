# Troubleshooting – GPO Application Failure

## Initial Symptoms
- User was still able to access Control Panel despite the policy being configured.

<img width="800" height="400" alt="Screenshot 2026-01-26 102016" src="https://github.com/user-attachments/assets/462f56a1-2dce-46df-95c9-9efa5d088f99" />

---

## Step 1: Review Applied Group Policies
- Ran gpresult to identify applied user policies.
- Confirmed the expected GPO was not listed.

<img width="800" height="400" alt="Screenshot 2026-01-26 104658" src="https://github.com/user-attachments/assets/6f9071c5-075e-43b8-b6a3-a6aa375c4aa3" />

---

## Step 2: Review GPO Scope
- Reviewed GPO link location in Group Policy Management.
- Identified that the GPO was linked to a computer OU while containing user configuration settings.

---

## Conclusion
The GPO did not apply due to incorrect OU linkage and scope mismatch.

