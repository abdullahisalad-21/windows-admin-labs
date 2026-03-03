🪟 Windows‑Admin — March 3, 2026
📘 Overview
Today I installed IIS on Windows using PowerShell and validated the installation through IIS Manager. I also analyzed the architectural differences between client Windows IIS and Windows Server IIS. Even though IIS installed successfully, I confirmed that Windows 10/11 does not include Server Manager or role‑based features, which explains why my interface did not match my tutor’s. This led to preparing for a Windows Server 2022 deployment, which is required for labs involving Server Manager, Add Roles and Features, DNS, DHCP, and enterprise‑grade IIS hosting.
🎯 Objectives
• Install IIS using PowerShell
 • Validate IIS components
 • Understand client vs server IIS differences
 • Prepare for Windows Server 2022 deployment
🛠️ Tools & Commands Used
Enable-WindowsOptionalFeature
IIS Manager
Windows Features panel
📝 Steps Completed
1. Installing IIS
I installed IIS using PowerShell and confirmed the installation.
2. Validating the Installation
I opened IIS Manager and verified that the management console was available.
3. Understanding OS Differences
I confirmed that Windows 10/11 does not include Server Manager roles, which explains the difference from my tutor’s environment.
4. Preparing for Windows Server
I prepared to download and install Windows Server 2022 to continue the lab with the correct environment.
🧩 Problems & Fixes
Problem: Missing Server Manager roles
 Fix: Identified OS limitation — requires Windows Server
📚 What I Learned
How IIS differs between Windows editions
Why Server Manager is only available on Windows Server
How to prepare a proper lab environment
🔗 Resources Used
PowerShell documentation
IIS documentation
