# PowerShell Defender Output

## Purpose

Capture Defender status using built-in PowerShell commands.

## Commands

Run PowerShell as administrator if needed:

```powershell
Get-MpComputerStatus
Get-MpPreference
```

## Evidence Captured

- Antivirus enabled
- Real-time protection enabled
- Antispyware enabled
- Signature age / update status
- Behavior monitoring status
- Device control and scan status fields visible in the captured output

## Screenshot Evidence

Captured screenshot:

`screenshots/02-defender-powershell-status.png`

## Redaction Notes

Blur or crop anything that exposes usernames, full local paths, organization names, device names, or policy details from an employer-managed device.
