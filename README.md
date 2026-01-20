# Ticket-Driven IT Support Simulation Lab

## Project Purpose
This project is a self-directed IT support simulation designed to demonstrate entry-level help desk and IT operations skills in a controlled lab environment.

Each ticket represents a realistic support scenario commonly handled by IT support technicians in Windows-based Active Directory environments. All scenarios were intentionally created, investigated, resolved, documented, and validated in a lab environment.

---

## Lab Environment
- Windows Server 2022 Domain Controller (AD DS + DNS)
- Windows 11 client machines
- Active Directory users, groups, and Group Policy
- File sharing using SMB
- Optional monitoring and log review

Environment Type: **Lab / Simulation**

---

## Ticket Workflow
Each ticket follows a consistent workflow:
1. Issue scenario is created in the lab
2. User symptoms are identified
3. Triage and diagnostics are performed
4. Root cause is identified
5. Resolution steps are applied
6. Fix is validated
7. Prevention or hardening steps are documented

Each ticket folder is fully self-contained and includes:
- The ticket record
- Scenario setup
- Troubleshooting steps
- Resolution and validation
- Prevention notes
- Supporting evidence (screenshots and logs)

---

## Repository Navigation
- Each folder named `Ticket-XX-*` represents one complete IT support case.
- Start with `01-ticket.md` inside any ticket folder for a high-level summary.
- Additional files provide deeper technical detail and evidence.

---

## Tools and Technologies Used
- Windows Server 2022
- Windows 11
- Active Directory Users and Computers (ADUC)
- Group Policy Management
- Event Viewer
- PowerShell
- Command-line troubleshooting tools (ipconfig, nslookup, gpresult, etc.)

---

## Realism and Integrity Statement
This project is a lab-based simulation created for learning and portfolio purposes only.

- All actions were performed in a controlled lab environment
- Scenarios reflect common real-world IT support tasks

---

## Key Skills Demonstrated
- Active Directory account management
- Troubleshooting authentication and access issues
- Group Policy analysis and remediation
- Windows networking fundamentals
- Endpoint support and remediation
- Clear technical documentation
- Root cause analysis and prevention-focused thinking
