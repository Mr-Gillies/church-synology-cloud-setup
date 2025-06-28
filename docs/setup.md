# Synology NAS Setup – The Bridge Church

This guide outlines the technical setup process for the Synology DS723+ NAS deployed at The Bridge Church. It includes storage initialization, shared folder creation, and data transfer procedures from a legacy LaCie drive.


1. Initial Configuration

NAS Access
- Navigated to [find.synology.com](https://find.synology.com) to locate the NAS on the local network
- Logged in using the administrator account: `setup-admin`
- Performed initial DSM setup on version 7.2

System Settings
- Set device name: `TheBridgeNAS`
- Configured admin user credentials
- Skipped enabling Synology Assistant visibility during setup (later confirmed enabled by default)


2. Drive and RAID Setup

Drive Information
- Installed 2× Seagate IronWolf 8TB NAS drives
- Selected **RAID 1** (mirrored setup) to ensure redundancy

Volume Creation
- Created a single volume (~7.2 TB usable)
- File system: **Btrfs** (for snapshot support and data integrity checks)
- Volume description: Local media cloud for multitracks, loops, and Ableton files

Screenshot Reference:
![RAID Setup](images/raid-setup.png)  
![Filesystem Selection](images/filesystem-selection.png)


3. Shared Folder Setup

- Created shared folder: `Lacie_2025_06`
- Enabled Recycle Bin
- Enabled file integrity protection
- Assigned `read/write` permissions to `setup-admin`
- `guest` account: No access

Screenshot Reference:
![Shared Folder Created](images/shared-folder-created.png)


4. Synology Drive Server

- Installed **Synology Drive Server** via Package Center
- Enabled the `Lacie_2025_06` folder as a Team Folder
- QuickConnect was preconfigured for external access (`bridgecloudnas`)


5. Data Migration

- Source: Legacy external LaCie drive
- Total migrated: ~1.6 TB
- Transfer performed via macOS Finder directly to NAS over LAN
- Folder structure preserved

Screenshot Reference:
![Physical LaCie Drive](images/physical-lacie-drive.jpeg)  
![Data Transfer Progress](images/data-transfer-progress.jpeg)


6. Deployment Status

- Device prepared and tested on a home network
- Ready for LAN integration at the church
- Admin handoff pending for static IP setup, backups, and user provisioning

Final Configuration View:
![Deployment Complete](images/final-connected-photo.jpg)


Notes

- No passwords, emails, or credentials are included in this file.
- All setup decisions were made to ensure flexibility and handoff readiness.





