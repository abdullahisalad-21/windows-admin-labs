# Windows Filesystem Repair & Disk Usage

## Overview
This documentation covers Windows NTFS filesystem repair, disk‑usage analysis, and Sysinternals DU.exe installation. The session focused on understanding NTFS self‑healing, TRIM optimization, and safe use of chkdsk.

## Objectives
- Learn NTFS self‑healing behavior  
- Practice disk‑usage commands  
- Install and use Sysinternals DU.exe  
- Understand why chkdsk requires reboot  
- Automate Disk Cleanup  

## Tools & Commands Used
- Get-PSDrive  
- Get-Volume  
- fsutil volume diskfree  
- fsutil repair query C:  
- cleanmgr /sageset:1  
- cleanmgr /sagerun:1  
- defrag C: /L  
- chkdsk /f  
- Sysinternals DU.exe  

## Steps Completed
1. Checked filesystem and disk usage  
2. Installed DU.exe manually and added to PATH  
3. Ran TRIM optimization  
4. Automated Disk Cleanup  
5. Queried NTFS self‑healing state (0x9)  
6. Attempted chkdsk /f and scheduled repair at reboot  

## Problems & Fixes
- **DU.exe not recognized** → Installed manually  
- **chkdsk cannot lock C:** → Scheduled at reboot  

## What I Learned
- NTFS repair modes (0, 1, 9, 0x10)  
- TRIM vs defrag  
- Disk Cleanup automation  
- Why system drives cannot be repaired while mounted  
- How DU.exe reports directory usage  

## Related Files
- DU.exe installation folder  
- chkdsk logs after reboot  

## Next Steps
- Review chkdsk results  
- Practice chkdsk /r on non‑system drives  
- Explore NTFS metadata repair  
