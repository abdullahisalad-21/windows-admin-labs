# 🪟 Windows Admin Labs — windows-hardening-2026-4-24.md

## 1. 🌅 Extended Overview
I reviewed Windows-specific hardening topics including BitLocker, UAC, AppLocker/WDAC, and patch management workflows.

## 2. 🎯 Objectives
- Understand BitLocker architecture and key protection.
- Learn how UAC enforces privilege separation.
- Review Windows patching workflows.
- Study application control on Windows endpoints.

## 3. 🛠️ Tools and Commands Used
- `manage-bde -status`
- BitLocker Group Policies
- AppLocker rule creation
- SCCM patch deployment

## 4. 📋 Steps Completed
- Reviewed TPM + PIN BitLocker configuration.
- Studied Secure Boot validation chain.
- Analyzed UAC elevation and admin token separation.
- Reviewed Windows Update channels and patch cycles.

## 5. 🐞 Problems and Fixes
- Clarified how BitLocker key rotation works without re-encrypting the disk.

## 6. 📚 What I Learned
- BitLocker protects against offline attacks and tampering.
- UAC prevents unauthorized privilege escalation.
- AppLocker/WDAC enforce strict application control.
- Patch management is critical for Windows fleet security.

## 7. 📎 Related Files
- Daily Practice 2026-4-24.md
- linux-hardening-2026-4-24.md

## 8. 🚀 Next Steps
- Build a BitLocker deployment plan.
- Create sample AppLocker policies for enterprise use.
