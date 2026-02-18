# 🪟 Resource Monitoring in Windows

## ⭐ 1. Overview
This documentation covers Windows resource monitoring using PowerShell, Task Manager, Resource Monitor, and Process Explorer. 
It explains how Windows exposes process information and how to inspect CPU and memory usage.

## 🎯 2. Objectives
- Understand Windows process and resource management  
- Use PowerShell to inspect CPU, memory, and process metadata  
- Analyze processes using Process Explorer  
- Compare GUI and CLI monitoring tools  

## 🛠️ 3. Tools & Commands Used

### 🧩 PowerShell
- `Get-Process`
- `Sort-Object`
- `Select-Object`
- `Stop-Process`

### 🖥️ GUI Tools
- Task Manager  
- Resource Monitor  
- Process Explorer  

## 🧪 4. Steps Completed
- Retrieved process information using:
  ```
  Get-Process
  ```
- Sorted processes by CPU usage:
  ```
  get-process | sort cpu -descending | select -first 3
  ```
- Identified high-memory processes:
  ```
  get-process | sort WS -descending | select -first 5
  ```
- Killed processes using:
  ```
  Stop-Process -Id <PID> -Force
  ```
- Analyzed Process Explorer:
  - CPU usage  
  - Working set  
  - Handles  
  - Threads  
  - DLLs  
  - Parent/child relationships  

## 🐞 5. Problems & Fixes
- ❗ Typo in PowerShell parameter → corrected `-firts` to `-first`  
- ❗ Process Explorer not in Start Menu → launched from Sysinternals folder  

## 📚 6. What I Learned
- `Get-Process` outputs `System.Diagnostics.Process` objects  
- PowerShell enables scriptable resource monitoring  
- Process Explorer provides deep visibility into process internals  
- Windows uses multiple layers of monitoring tools  

## 📎 7. Related Files
- PowerShell screenshots  
- Process Explorer screenshots  

## 🔜 8. Next Steps
- Document PerfMon counters  
- Explore WPR/WPA  
- Build PowerShell monitoring cheat sheet  
