# Active Directory Architecture — Module 4 Concepts

## 1. Administrative Groups
- Enterprise Admins: forest-wide authority.
- Domain Admins: domain-wide authority.
- Domain Controllers: DC computer accounts.
- Domain Computers: all domain-joined machines.
- Domain Users: standard user accounts.

## 2. Multi-Domain Forest Design
- Forest = security boundary.
- Automatic two-way transitive trusts.
- Shared schema and global catalog.
- Forest root domain holds Enterprise Admins and Schema Admins.

## 3. AGUDLP Model
Accounts → Global Groups → Universal Groups → Domain Local Groups → Permissions.

## 4. Group Scope
- Domain Local: assign permissions.
- Global: represent users.
- Universal: forest-wide grouping.

## 5. AD Functional Levels
### 2012 R2:
- Protected Users.
- Authentication policies and silos.

### 2016:
- PAM.
- DFSR-only SYSVOL.
- Kerberos PKInit Freshness.

### 2025:
- 32k NTDS database pages.

## 6. Screenshot Analysis
Your account = Domain Users only → standard user privileges.
