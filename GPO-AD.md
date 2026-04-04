# 1. Overview ⭐
Today I completed a full GPO and AD practical session: creating GPOs, editing them, linking them, understanding inheritance and precedence, and performing GPO troubleshooting (Parts 1 & 2). I also validated AD health and authentication.

# 2. Objectives 🎯
- Create and edit GPOs
- Understand GPO linking and scope
- Practice inheritance, precedence, enforcement, block inheritance
- Perform GPO troubleshooting using GPMC and gpresult
- Validate AD authentication and DNS
- Complete an AD practical test

# 3. Tools & Commands Used 🛠️
- GPMC
- Group Policy Results Wizard
- gpresult /r and /h
- gpupdate /force
- Resolve-DnsName
- whoami /all
- Active Directory Users & Computers

# 4. Steps Completed 🧩
## A. GPO Creation & Editing
- Created new GPOs for user and computer settings
- Edited policies (security, scripts, preferences)
- Linked GPOs to OUs

## B. Inheritance & Precedence
- Practiced LSDOU order
- Adjusted link order
- Tested enforced GPOs
- Tested block inheritance
- Observed how precedence overrides lower-level GPOs

## C. Troubleshooting (Part 1 & 2)
- Verified DNS and SRV records
- Checked logon server
- Diagnosed cached credentials
- Used GPMC to generate RSoP
- Identified filtering, delegation, WMI issues
- Validated SYSVOL/NETLOGON access

## D. AD Practical Test
- Verified domain join
- Tested authentication
- Checked replication (single DC environment)
- Confirmed GPO application on client

# 5. Problems & Fixes 🐞
- GPO not applying due to cached credentials → fixed by DNS correction + reboot
- Incorrect GPO scope → corrected by linking to proper OU

# 6. What I Learned 📚
- GPO processing order determines final applied settings
- Enforcement overrides block inheritance
- Security filtering requires Read + Apply permissions
- GPMC provides deeper insights than gpresult
- AD authentication directly affects GPO processing

# 7. Related Files 📎
- None generated today

# 8. Next Steps 🔜
- Create more complex GPOs
- Test WMI-filtered GPOs
- Practice loopback processing scenarios
