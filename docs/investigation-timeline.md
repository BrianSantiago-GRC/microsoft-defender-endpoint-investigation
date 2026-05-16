# Investigation Timeline

## Purpose

Create a simple analyst timeline showing what was checked and why.

| Step | Time | Action | Evidence | Result |
|---:|---|---|---|---|
| 1 | 2026-05-15 | Reviewed Windows Security / Defender status | `screenshots/01-windows-security-defender-status.png` | No current threats shown; Defender status visible. |
| 2 | 2026-05-15 | Captured Defender PowerShell status | `screenshots/02-defender-powershell-status.png` | Defender and antivirus status values captured; ComputerID redacted. |
| 3 | 2026-05-15 | Reviewed Event Viewer Security log | `screenshots/03-event-viewer-security-log.png` | Security audit log view captured. No username, domain, or device identifier is visible in the screenshot. |
| 4 | 2026-05-15 | Reviewed System log evidence | `screenshots/04-event-viewer-system-or-application-log.png` | System log evidence captured with Service Control Manager event context. |
| 5 | 2026-05-15 | Wrote containment/remediation recommendations | `docs/remediation-recommendations.md` | Recommendations drafted for Defender status, log review, escalation, and documentation. |

## Screenshot Evidence

Rendered timeline screenshot:

`screenshots/05-investigation-timeline.png`
