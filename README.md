# Church Synology Cloud Setup

This repository documents the full deployment and staging process of a Synology NAS solution designed to serve The Bridge Church. This system was created to replace aging storage workflows and introduce secure, LAN-accessible, and resilient storage for the Worship Arts Department.

The goal was to implement a solution that bridges local and remote workflows while keeping integration simple for IT professionals, musicians, and creative staff alike.


## Why This Was Built

- To organize and centralize the church's worship-related media  
- To transfer content from an aging 1.6TB LaCie external drive  
- To create a reliable and redundant local storage system  
- To introduce internal cloud storage with optional mobile/web access  
- To stage a system ready for secure handoff to IT for final networking and VLAN assignment  


## System Overview

| Component             | Details                              |
|----------------------|--------------------------------------|
| **NAS Model**        | Synology DS723+                      |
| **Drives**           | 2× 8TB Seagate IronWolf (RAID 1)     |
| **Total Usable Storage** | ~7.2 TB                          |
| **File System**      | Btrfs                                |
| **Main Shared Folder** | `Lacie_2025_06`                    |
| **Remote Access**    | QuickConnect configured              |
| **Deployment Status**| Physically installed, awaiting network integration |


## Project Folder Structure

```

church-synology-cloud-setup/
├── README.md
├── .gitignore
├── setup.md
├── IT-deployment-overview.md
├── docs/
│   └── images/
│       ├── 1. Hardware Assembly Synology NAS.png
│       ├── 2. Assembled and configured at home.png
│       ├── 3. Physical Lacie Drive.png
│       ├── bridge-nas-installed-unplugged.jpg
│       ├── Config 1.png
│       ├── Config 2.png
│       ├── Config 3.png
│       ├── Config 4.png
│       ├── Config 5.png
│       ├── Config 6.png
│       └── Lacie Data Transfer.png

```



## What's Inside

- `setup.md`: Step-by-step documentation of the RAID config, shared folder creation, encryption, and upload process  
- `IT-deployment-overview.md`: A handoff-ready summary document for IT integration and credentials  
- `images/`: Screenshots and documentation of hardware placement, DSM setup, and drive transfer steps  


## What is Completed

- ✅ Synology DS723+ hardware configured and labeled as "BridgeNAS"  
- ✅ RAID 1 setup for full drive redundancy  
- ✅ Filesystem selected as Btrfs for advanced data integrity protection  
- ✅ Synology Drive Server and Photos evaluated (not actively configured)  
- ✅ Shared folder `Lacie_2025_06` created with:  
  - MixedAudioFiles  
  - Multitracks  
  - Planning Center Click Tracks  
  - Archived `.als` sessions for Ableton  
- ✅ Legacy LaCie drive (1.6 TB) fully cloned to NAS  
- ✅ NAS successfully placed in church server rack (not plugged in)  
- ✅ Remote access enabled via QuickConnect (`bridgecloudnas`)  
- ✅ Final photo added of NAS in rack with network cable unplugged (Notified our IT team through our communication software: Trello)
- ⬜ Final IP setup, VLAN mapping, and secure access control to be handled by IT  


## Notes for Reviewers

- Security policies (firewall rules, static IP reservations, VPN access) were left untouched to avoid interference with Dante, VLAN, or LAN setups  
- Device is not yet on the network — network connection and VLAN assignment will be completed by the IT team  
- Unit was fully staged and tested on a secure home network prior to delivery  


## Future Considerations

Multitrack organization and `.als` file routing are scheduled for reformatting to align with:

- M32/X32 digital console workflows  
- Dante Controller routes  
- Unified Ableton Live session templates for worship  

These improvements will be led by Art Fuller and Ryan Gillies during the next phase post-network integration  


## Final Comments

This repository contains no credentials or sensitive information. It is purely for documentation, reproducibility, and IT handoff clarity. Internal passwords and access control are handled outside GitHub.

This project was developed with security, accessibility, and long-term handoff in mind.

**Maintainer:** Ryan Gillies
