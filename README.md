# Windows Defender Endpoint Review

**A Windows endpoint-posture and evidence-collection walkthrough built from an IT support investigation sequence.**

## Problem, Action, Result

**Problem:** A user report or endpoint concern needs a quick, defensible baseline before an analyst can decide whether to remediate, escalate, or collect more evidence.

**Action:** I checked Windows Security status, captured `Get-MpComputerStatus` output, reviewed Event Viewer surfaces, and organized the work into an analyst timeline and remediation checklist.

**Result:** The repository shows a repeatable endpoint-review sequence and clear handoff documentation. The captured system showed no active threat; this is not a claim that malware was found, contained, or eradicated.

## 90-Second Review

1. Inspect the [Windows Security status](screenshots/01-windows-security-defender-status.png).
2. Review the [`Get-MpComputerStatus` evidence](evidence/powershell-output.md).
3. Read the [Event Viewer review](evidence/event-viewer-review.md).
4. Follow the [investigation timeline](docs/investigation-timeline.md) and [remediation recommendations](docs/remediation-recommendations.md).

## Evidence Map

| Evidence | What it shows | Boundary |
|---|---|---|
| [Windows Security](screenshots/01-windows-security-defender-status.png) | Built-in endpoint protection status | Posture check, not an EDR alert |
| [PowerShell status](screenshots/02-defender-powershell-status.png) | Defender configuration and health fields | Point-in-time local output |
| [Security event log](screenshots/03-event-viewer-security-log.png) | Windows Security log review surface | No malware event is claimed |
| [System/Application log](screenshots/04-event-viewer-system-or-application-log.png) | Supporting event-review surface | Context gathering, not root-cause proof |
| [Timeline](screenshots/05-investigation-timeline.png) | Rendered Markdown investigation sequence | Documentation artifact, not a live incident console |
| [Recommendations](screenshots/06-remediation-recommendations.png) | Rendered action and escalation checklist | Proposed steps, not completed containment |

## Skills Demonstrated

Windows 10/11 | Windows Security | Microsoft Defender Antivirus | PowerShell | Event Viewer | endpoint triage | evidence capture | escalation notes | remediation planning | technical documentation

## Scope Boundary

This project uses built-in Windows and Defender Antivirus evidence. It does not demonstrate Microsoft Defender for Endpoint administration, live EDR alert triage, malware reverse engineering, threat hunting, or production incident containment.

## Interview Summary

> I used a support-first sequence: confirm endpoint protection status, capture PowerShell health data, review relevant Windows logs, separate observed facts from assumptions, and document the next action. The system showed no active threat, so I treated the result as a posture baseline rather than inventing an incident.
