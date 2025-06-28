# Synology NAS Deployment Overview – The Bridge Church

This document outlines the deployment process and technical configuration for a self-hosted Synology NAS system used by The Bridge Church. This local cloud solution provides centralized access to multitrack files, Ableton sessions, media archives, and general documentation.


1. Project Goals

- Enable internal access to critical worship and media assets
- Replace reliance on third-party cloud services
- Provide local, LAN-accessible storage for staff and volunteers
- Allow future growth and administrative flexibility via Synology DSM


2. Hardware & Configuration

- **NAS Model:** Synology DS723+
- **Drives:** 2x Seagate IronWolf NAS 8TB (RAID 1)
- **RAID Type:** RAID 1 (mirrored for redundancy)
- **Volume:** ~7.4 TB allocated for media
- **File System:** Btrfs for advanced snapshot and data protection features


3. Shared Folders

- **Primary Folder:** `Lacie_2025_06`
  - **Purpose:** Archive of audio projects, multitrack exports, and loops
  - **Recycle Bin:** Enabled
  - **Permissions:** Managed via DSM


4. Access Options

- **Local Access:** Mapped as network share on Windows/macOS
- **Remote Access:** QuickConnect configured
- **DSM Access:** Browser login interface for administrators


5. Deployment Notes

- The NAS has been initialized and tested on a home network
- Ready to be connected to the church’s LAN via Ethernet
- Data transfer (1.6 TB) from legacy drive has been completed
- Admin accounts and folders are structured but flexible

6. Visual References

Screenshots of the setup process and data migration are included in the `docs/images/` folder of this repository to provide reference for future maintenance or auditing.


Maintained By

This setup was prepared with future scalability and IT oversight in mind. Handoff to the church's IT lead is advised for final integration, access control, and backup policy.

