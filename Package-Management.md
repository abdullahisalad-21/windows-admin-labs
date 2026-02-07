# ✅ **3. windows-admin-lab-2026-02-07.md**

```markdown
# Windows Admin Lab — Package Management

## Overview
This lab covered Windows package management using PowerShell, NuGet providers, and winget. I practiced searching for packages, installing providers, and understanding dependency behavior in Windows.

---

## Commands / Work Done
```powershell
Find-Package sysinternals -IncludeDependencies
• 	Installed NuGet provider when prompted.
• 	Compared Windows  with Linux  installation.

What I Learned
• 	PowerShell requires the NuGet provider to search PSGallery.
• 	Provider download failures occur due to network or TLS issues.
• 	Windows uses centralized repositories, making installation simpler.
• 	Winget automatically resolves dependencies.

Scenarios
• 	Troubleshooting PowerShell provider errors.
• 	Installing SysInternals tools.
• 	Comparing Windows and Linux package ecosystems.
