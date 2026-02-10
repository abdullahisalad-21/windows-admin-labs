🧩 1. Overview
Today’s Windows lab covered:
• 	FAT32 vs NTFS
• 	MBR vs GPT
• 	Disk partitioning essentials
• 	Selecting disks (Disk 0)
• 	Creating primary partitions
• 	Formatting partitions (NTFS/FAT32)
• 	Mounting and unmounting volumes
• 	Reading supplemental materials
This was a complete introduction to Windows storage fundamentals.
🎯 2. Objectives
• 	Understand Windows filesystem types
• 	Learn the difference between MBR and GPT
• 	Practice partitioning workflows
• 	Understand how Windows formats and mounts volumes
• 	Build foundational disk management knowledge
🛠️ 3. Tools & Concepts Used
Disk Management Concepts
• 	Disk 0 (system disk)
• 	Primary partitions
• 	Filesystem selection
• 	Volume mounting
• 	Volume formatting
Filesystems
• 	FAT32
• 	Simple
• 	Highly compatible
• 	Max file size 4GB
NTFS
- Modern
- Supports permissions
- Journaling
- Required for Windows system drives
Partition Table Types
MBR
- Legacy
- 4 primary partitions
- 2TB limit
GPT
- Modern
- Required for UEFI
- Supports large disks
Reading Materials
- Disk Partition and Filesystem Essentials
- MBR vs GPT
- Mounting and Unmounting Filesystems
- FAT32 vs NTFS
🧱 4. Steps Completed
4.1 Understanding Filesystems
You reviewed:
• 	Why NTFS is used for Windows
• 	Why FAT32 is used for USB drives
• 	How journaling works
• 	How filesystem choice affects performance and compatibility
4.2 Understanding Partition Tables
You learned:
- Why GPT is the modern standard
- Why MBR is limited
- How Windows uses GPT for UEFI systems
4.3 Disk Partitioning Workflow
You practiced the conceptual workflow:
- Select disk (Disk 0)
- Create primary partition
- Choose filesystem (NTFS or FAT32)
- Format the partition
- Assign drive letter
- Mount the volume
- Unmount when needed
4.4 Formatting Partitions
  I reviewed:
• 	Formatting into NTFS
• 	Formatting into FAT32
• 	When each filesystem is appropriate
📘 5. What I Learned
• 	How Windows structures disks
• 	Why GPT is preferred
• 	How NTFS differs from FAT32
• 	How to create and format partitions
• 	How Windows mounts/unmounts volumes
• 	How partition tables affect booting and storage
🚀 6. Next Steps
• 	Practice using Disk Management GUI
• 	Practice using diskpart
• 	Explore NTFS permissions
• 	Compare Windows vs Linux filesystem behavior
