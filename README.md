### Church Synology Cloud Setup:

This project documents the setup and deployment of a Synology NAS system at The Bridge Church. The goal was to move away from relying on external hard drives and cloud platforms by setting up a secure, centralized storage solution that volunteers and staff can access internally.

Everything was planned with the future in mind — this setup keeps things clean, simple, and scalable for whoever takes over next.


Why This Was Built:

- To organize and centralize the church's worship-related media
- To transfer content from an aging LaCie external drive into a reliable system
- To create a local cloud setup that integrates well with our network
- To set things up in a way that doesn’t interfere with existing IT systems


System Overview:

| Component             | Details                              |
|----------------------|--------------------------------------|
| NAS Model            | Synology DS723+                      |
| Drives               | 2× 8TB Seagate IronWolf (RAID 1)     |
| Total Usable Storage | ~7.2 TB                              |
| File System          | Btrfs                                |
| Main Shared Folder   | `Lacie_2025_06`                      |
| Remote Access        | QuickConnect configured              |
| Deployment Status    | Staged and ready for LAN integration |


Project Folder Structure:

``` 
church-synology-cloud-setup/
├── README.md
├── .gitignore
├── docs/
│   ├── setup.md
│   ├── IT-deployment-overview.md
│   └── images/
│       ├── raid-setup.png
│       ├── filesystem-selection.png
│       ├── shared-folder-created.png
│       ├── physical-lacie-drive.jpeg
│       ├── data-transfer-progress.jpeg
│       └── final-connected-photo.jpg
```


What’s Inside:

- [`setup.md`](docs/setup.md): Detailed walkthrough of RAID setup, shared folder configuration, and data migration process
- `IT-deployment-overview.md`: Clean, high-level summary for future handoff
- `images/`: Screenshots from the setup process and physical install


What’s Done So Far:

- [x] NAS set up and tested on home network
- [x] RAID 1 configured for drive redundancy
- [x] Folder created and permissions applied
- [x] 1.6 TB transferred from LaCie drive
- [x] Remote access enabled
- [ ] Final handoff and LAN setup by IT team


Notes:

Everything here was built with care and intention to support the church moving forward. This repo does not contain passwords or internal credentials — only public documentation and visuals related to the project setup.

