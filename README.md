# Ticket-Driven IT Support Simulation Lab

## Start Here — Quick Highlights

If you only review a few tickets, start with these for maximum impact:

- **Ticket 04** – Shared Folder Permission Issue (NTFS vs Share)
- **Ticket 06** – Group Policy Not Applying
- **Ticket 10** – Client Unable to Resolve Internal DNS Names
- **Ticket 13** – User Logging In With Temporary Profile
- **Ticket 19** – Accidental Deletion of AD User Object (Recovery)

---

## Project Purpose

This repository is a **self-directed, lab-based IT Support simulation** designed to demonstrate real-world troubleshooting, documentation, and resolution workflows commonly handled by **Entry-Level IT Support / Help Desk Technicians** in Windows-based Active Directory environments.

The focus of this project is not automation or scripting alone, but **structured ticket handling**, including:
- Triage
- Root cause analysis
- Resolution
- Validation
- Prevention and escalation awareness

All scenarios are intentionally designed to reflect **realistic issues**, not artificial lab exercises.

---

## Lab Environment Overview

**Domain Environment**
- Domain: `lab.local`
- Domain Controller: Windows Server 2022 (`SRV-CORE01`)
- Services: Active Directory Domain Services, DNS
- IP Addressing: Static (lab constraint)

**Client Systems**
- Windows 11 Pro domain-joined clients
- Multiple workstations used to simulate user impact

**Infrastructure Notes**
- Lab-only environment
- No production claims
- No enterprise ownership implied

---

## Ticket Workflow Used

Each ticket follows a consistent structure to mirror real IT service workflows:

1. **Scenario** – What the user reported / what triggered the ticket  
2. **Troubleshooting** – Tools, checks, and reasoning used  
3. **Resolution** – Step-by-step fix  
4. **Validation** – How the fix was confirmed  
5. **Prevention** – How recurrence could be reduced  
6. **Escalation Notes** – When this would be escalated in a real job  

Evidence (screenshots/logs) is embedded **directly within the narrative** to preserve context.

---

## Repository Structure
```text
it-ticket-sim-lab/
├── README.md
├── tickets/
│ ├── Ticket-01-Account-Lockout/
│ ├── Ticket-02-Password-Reset/
│ ├── ...
│ └── Ticket-20-File-Restore-From-Backup/
```


Each ticket folder contains:
- `01-ticket.md` – Ticket summary
- `02-scenario.md`
- `03-troubleshooting.md`
- `04-resolution.md`
- `05-prevention.md`

---

## Tools & Technologies Used

- **Windows Server 2022**
  - Active Directory Domain Services
  - DNS
  - Group Policy Management
- **Windows 11 Pro**
  - Domain-joined client troubleshooting
- **Active Directory Users & Computers**
- **Group Policy Management Console**
- **Event Viewer**
  - Security, System, and Application logs
- **Command-Line Tools**
  - `ipconfig`, `nslookup`, `ping`, `gpresult`, `w32tm`
- **PowerShell**
  - Account checks, service verification, system validation

---

## How to Evaluate This Repository

For reviewers or hiring managers:

1. Start with the **Ticket Summary (`01-ticket.md`)** for any ticket.
2. Review troubleshooting steps to understand diagnostic thinking.
3. Check resolution and validation for correctness and safety.
4. Observe prevention notes for operational maturity.
5. Tickets increase in complexity as numbering increases.

---

## Who This Project Is For

This project is intended to demonstrate readiness for roles such as:
- IT Support Technician
- Help Desk Analyst
- Desktop Support Specialist
- Junior Systems Administrator

It emphasizes **clear communication**, **methodical troubleshooting**, and **safe remediation** over theoretical knowledge alone.

---

## Realism Statement

All work in this repository was performed in a **personal lab environment** for educational and portfolio purposes only.

- No production systems were used
- No enterprise authority is implied
- Scenarios are simulations based on real-world IT support patterns

---

## Key Skills Demonstrated

- Active Directory account lifecycle management
- Group Policy troubleshooting and optimization
- DNS and network connectivity isolation
- NTFS and share permission analysis
- Endpoint troubleshooting (profiles, updates, storage)
- Log analysis and monitoring awareness
- Backup and recovery fundamentals
- Documentation suitable for handoff and escalation

---

## Full Ticket Index

- Ticket 01 – Account Lockout
- Ticket 02 – Password Reset With Forced Change
- Ticket 03 – New User Onboarding
- Ticket 04 – Shared Folder Permission Issue
- Ticket 05 – User Access Removed Incorrectly
- Ticket 06 – Group Policy Not Applying
- Ticket 07 – Network Drive Mapping via GPO Fails
- Ticket 08 – GPO Causes Login Delay
- Ticket 09 – Security Policy Change Causes Login Failure
- Ticket 10 – Client Unable to Resolve Internal DNS Names
- Ticket 11 – User Cannot Access File Server
- Ticket 12 – VPN Client Unable to Connect
- Ticket 13 – Temporary User Profile Issue
- Ticket 14 – Disk Space Alert on Client Machine
- Ticket 15 – Windows Update Failing on Client
- Ticket 16 – Multiple Failed Login Attempts Detected
- Ticket 17 – Critical Windows Service Stopped
- Ticket 18 – Authentication Failures Due to Time Sync Issue
- Ticket 19 – Accidental Deletion of AD User Object
- Ticket 20 – File Restore From Backup After Accidental Deletion
