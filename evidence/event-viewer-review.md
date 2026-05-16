# Event Viewer Review

## Purpose

Document basic Windows log review as endpoint investigation evidence.

## Logs To Review

- Windows Logs > Security
- Windows Logs > System
- Windows Logs > Application

## Useful Event Examples

| Event ID | Meaning |
|---:|---|
| 4624 | Successful logon |
| 4625 | Failed logon |
| 4634 | Logoff |
| 4688 | Process creation, if auditing is enabled |
| 7045 | Service installed |
| 7036 | Service state changed |

## Screenshot Evidence

Captured screenshots:

- `screenshots/03-event-viewer-security-log.png`
- `screenshots/04-event-viewer-system-or-application-log.png`

## Review Notes

Focus on showing you know where to look, how to capture evidence, and how to explain why a log matters. Do not claim incident response ownership or advanced forensic analysis.
