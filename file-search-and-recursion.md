# File Search and Recursion in PowerShell

## Searching for files
Get-ChildItem -Recurse -Filter "*.txt"

## Searching inside files
Select-String -Pattern "error" -Path *.log

## What I Learned
- How to search recursively  
- How to filter by file type  
