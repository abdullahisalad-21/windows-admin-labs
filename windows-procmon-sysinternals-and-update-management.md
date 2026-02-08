
```markdown
# Windows ProcMon, Sysinternals, and Update Management – 2026-02-08

## Overview
Today’s Windows admin session focused on Windows Update fundamentals, Sysinternals tools, and process-level diagnostics.
I practiced discovering, installing, and launching Process Monitor and Process Explorer using PowerShell, explored resource monitoring tools, and analyzed real-time system activity.
This session strengthened my understanding of Windows servicing, troubleshooting, and low-level system behavior.

---

## Commands / Work Done

### Sysinternals Installation (PowerShell)
```powershell
install-package -name sysinternals

Discovering and Installing ProcMon via Winget
winget search procmon
winget install --id Microsoft.Sysinternals.ProcessMonitor

Running Sysinternals Tools
procmon
procexp
resmon
Running ProcMon from Full Path
& "C:\Program Files\Sysinternals\Procmon.exe"
Optional PATH Extension
setx PATH "$env:PATH;C:\Program Files\Sysinternals" /M

What I Learned
Windows Update Concepts
• 	Windows Update delivers security, quality, feature, and driver updates.
• 	Updates can be managed locally or centrally (Group Policy, WSUS, Intune).
• 	Regular updates maintain system security and stability.
• 	Feature updates introduce major OS changes; quality updates fix bugs and improve reliability.
Sysinternals Tools
• 	Process Monitor (ProcMon) captures low-level file, registry, and process events.
• 	Process Explorer (procexp) provides high-level process insights (CPU, memory, handles, DLLs).
• 	resmon (Resource Monitor) shows real-time CPU, disk, network, and memory usage.
• 	Sysinternals tools do not always create terminal aliases; some require full path execution.
• 	Filtering in ProcMon is essential for meaningful analysis.
ProcMon Event Types
- File operations: CreateFile, ReadFile, WriteFile.
- Registry operations: RegOpenKey, RegQueryValue, RegSetValue.
- Result states: SUCCESS, NAME NOT FOUND, ACCESS DENIED
Diagnosing a Failing Windows Installer
1. 	Launch ProcMon.
2. 	Apply filters:
• 	Process Name is msiexec.exe
• 	Result is Access Denied 
3. 	Identify missing files, denied registry keys, or permission issues.
4. 	Use findings to adjust permissions or repair installer components.

