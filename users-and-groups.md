# Windows Users and Groups

## Listing Users
Get-LocalUser

## Creating Users
net user john Password123 /add

## Listing Groups
Get-LocalGroup

## Adding User to Group
Add-LocalGroupMember -Group "Administrators" -Member "john"

## What I Learned
- How Windows stores local accounts  


## Scenario: Resetting a locked account

A user forgot their password and was locked out.  
I used:

net user john NewPass123

Then I forced a password change at next login:

net user john /logonpasswordchg:yes

This restored access securely.
