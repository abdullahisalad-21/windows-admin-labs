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
