# Troubleshooting – Login Performance Issue

## Initial Symptoms
- User login completed successfully but experienced a noticeable delay during “Applying user settings.”
- No authentication failures or error messages were observed.

---

## Step 1: Review Applied Group Policies
- Ran `gpresult /r` on the affected workstation.
- Confirmed multiple user-scoped Group Policy Objects were applied, including the newly created desktop restriction policy.

<img width="800" height="400" alt="Screenshot 2026-01-27 114840" src="https://github.com/user-attachments/assets/a2a32a7e-1235-4b23-9697-1b20f3d866f2" />

---

## Step 2: Review GPO Scope
- Reviewed the link location of the newly created GPO in Group Policy Management.
- Identified that the policy was linked at a high-level OU, causing it to be processed for all users during logon.

<img width="400" height="400" alt="Screenshot 2026-01-27 114646" src="https://github.com/user-attachments/assets/a503d3c7-a47b-441a-8a3a-d0ffd861586b" />

---

## Analysis
- Client-side tools such as `gpresult` confirm whether a policy applies but do not reflect overall GPO scope.
- Broadly scoped user policies increase cumulative logon processing time even when functionality remains correct.

---

## Conclusion
Login delays were caused by unnecessary processing of user policies due to overly broad GPO scope.
