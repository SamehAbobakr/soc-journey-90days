
# Task 03: Windows Event Log Analysis

## Objective
Learn how to analyze Windows Event Logs and investigate security-related activities.

## Learning Objectives
- Understand Windows Security Event IDs.
- Identify different Windows Logon Types.
- Analyze successful and failed login attempts.
- Detect user account creation and privilege changes.
- Use PowerShell Get-WinEvent to investigate Windows logs.
- Build an event timeline from collected evidence.

## Event IDs
4624 - Successful Logon
4625 - Failed Logon
4634 - Logoff
4648 - Explicit Credentials
4672 - Special Privileges Assigned
4688 - Process Creation
4720 - User Account Created
4732 - Member Added to Security Group
1102 - Security Audit Log Cleared
7045 - New Service Installed

## Practical Lab
- Enable Windows Audit Policies.
- Generate failed and successful login events.
- Create a test user.
- Add the test user to the Administrators group.
- Export and analyze relevant EVTX events.

## Deliverables
- event-id-cheatsheet.md
- timeline.md
- Evidence files and screenshots

## Completion Criteria
- Analyze at least 5 events in a chronological timeline.
- Achieve at least 70% in the knowledge assessment.


