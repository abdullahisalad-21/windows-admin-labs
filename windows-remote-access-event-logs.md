**✅ WINDOWS‑ADMIN LABS — Documentation
🗂️ Overview**
Today I practiced Windows remote access, PowerShell remoting, log monitoring, and virtualization management as part of Module 6. 
I used RDP, PowerShell remote commands, and Event Viewer to understand system behavior.
I managed Windows virtual machines inside VirtualBox to simulate real admin workflows.
**🎯 Objectives**
• 	Remotely access Windows systems using RDP
• 	Execute administrative tasks through PowerShell remoting
• 	Analyze Windows logs for troubleshooting and system health
• 	Manage Windows VMs, snapshots, and states in VirtualBox
• 	Strengthen Windows admin fundamentals through hands‑on practice.
**🛠️ Tools & Commands Used**
- RDP (Remote Desktop Protocol)
- PowerShell Remoting
- Event Viewer
- VirtualBox (Windows VM)
- PowerShell commands:
- Enter-PSSession
- Invoke-Command
- Get-EventLog
- Get-WinEvent
**🧩 Steps Complete**d
• 	Connected to a Windows machine using RDP for remote GUI administration
• 	Executed remote PowerShell commands to manage the system without GUI
• 	Reviewed Event Viewer logs (System + Application)
• 	Identified key Event IDs related to authentication, system health, and errors
• 	Created custom Event Viewer filters to isolate relevant logs
• 	Managed Windows VM snapshots, states, and rollbacks in VirtualBox
• 	Practiced switching between GUI‑based and CLI‑based administration.
**🐞 Problems & Fixes**
• 	RDP login issues — Verified credentials, checked network reachability, ensured RDP was enabled
• 	PowerShell remoting errors — Enabled WinRM, configured trusted hosts, confirmed firewall rules
• 	Event Viewer clutter — Used filtering by Event ID, log type, and timestamp to isolate useful data
• 	VM state inconsistencies — Restored snapshots and reconfigured VM settings to stabilize the environment.
**📘 What I Learned**
• 	RDP is a core tool for remote Windows administration, especially for GUI‑based tasks
• 	PowerShell remoting provides deeper, faster, and more scalable control than GUI tools
• 	Event Viewer is essential for diagnosing Windows issues, crashes, authentication failures, and system health
• 	VirtualBox offers a safe environment to test Windows admin tasks without risking production systems
• 	Combining RDP, PowerShell, and Event Viewer creates a complete troubleshooting workflow
• 	Snapshots are critical for safe experimentation and rollback during labs.
🚀 Next Steps
• 	Configure WinRM for advanced PowerShell remoting scenarios
• 	Practice remote troubleshooting across multiple Windows VMs
• 	Explore Windows OS deployment tools (WDS, MDT, Sysprep)
• 	Build automated log‑collection scripts using PowerShell
• 	Document more real‑world remote‑admin scenarios for the portfolio. 
