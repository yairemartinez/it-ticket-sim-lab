# Troubleshooting – Authentication Failure

## Initial Symptoms
- User reported authentication-related access issues.
- No account lockouts or credential changes were observed.

---

## Step 1: Verify Account Status
- Confirmed the user account was enabled and not locked.
- Verified no recent password resets or policy changes.

---

## Step 2: Review System Time Configuration
- Verified domain controller system time on SRV-CORE01.
- Verified client system time on WIN11-02.
- Confirmed domain policies enforced time synchronization on the client.

---

## Step 3: Review Kerberos Ticket State
- Reviewed Kerberos tickets on the client using `klist`.
- Confirmed valid Kerberos tickets were present.
- No evidence of ticket rejection or expiration due to time skew.

---

## Step 4: Validate Access Behavior
- Confirmed access failures were permission-related rather than authentication-related.
- Verified failures were consistent with group membership restrictions.

---

## Conclusion
Time drift was investigated as a potential cause but was ruled out based on system time verificat
