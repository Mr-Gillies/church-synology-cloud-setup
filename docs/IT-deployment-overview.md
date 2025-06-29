# Synology NAS Deployment Overview – The Bridge Church

This document outlines the deployment and configuration of a self-hosted Synology NAS system implemented for The Bridge Church. The solution provides centralized LAN-accessible storage for multitracks, Ableton sessions, worship media, and internal documentation.

---


1. Project Goals

- Provide internal access to critical worship and media assets
- Replace reliance on third-party cloud solutions
- Support staff and volunteer workflows through centralized, reliable storage
- Allow future administrative flexibility using Synology DSM


2. Hardware & Configuration

- **NAS Model:** Synology DS723+
- **Drives:** 2× Seagate IronWolf NAS 8TB
- **RAID Type:** RAID 1 (mirrored for redundancy)
- **Volume Size:** ~7.2 TB usable
- **File System:** Btrfs (for snapshots, integrity protection, and advanced file control)


3. Shared Folder Structure

- **Primary Folder:** `Lacie_2025_06`
  - **Contents:** Audio projects, multitrack exports, loops, and archived Ableton sessions
  - **Recycle Bin:** Enabled
  - **Permissions:** Controlled via DSM admin interface


4. Access Options

- **Local Network Access:** Mappable as a shared drive on Windows/macOS
- **Remote Access:** Configured via Synology QuickConnect (internal access ID available on request)
- **DSM Access:** Synology Drive and DSM interface are enabled, but access details are managed internally



5. Deployment Status

- ✅ NAS initialized, staged, and tested on secure home network
- ✅ RAID 1 configured and verified
- ✅ 575.68 GB of media transferred from legacy LaCie external drive
- ✅ Placed in church’s existing equipment rack
- ⬜ Network cable left unplugged to avoid interrupting existing VLAN, Dante, or LAN systems (Notified IT Team through our Trello board)
- ⬜ Final network integration, VLAN mapping, and IP reservation to be completed by IT professional


6. Visual References

Setup screenshots and photos of hardware placement are located in:


Refer to these files for visual verification of each configuration step and the physical rack install.

---

## Maintainer Notes

This deployment was structured to be non-intrusive and safe for integration into an existing production network. All security, firewall, and access policies are to be finalized by the church’s IT lead.

> Maintained by: **Ryan Gillies**

For future multitrack and Ableton `.als` session refinement, coordination will be handled by **Art Fuller** and **Ryan Gillies**.

