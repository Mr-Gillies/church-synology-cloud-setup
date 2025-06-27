# Synology Cloud Setup – The Bridge Church

This document outlines the setup of a self-hosted cloud system using a Synology DS723+ NAS. The solution is designed for internal media storage, volunteer access, and document management at The Bridge Church.

---

## 1. Hardware Overview

- NAS Model: Synology DS723+
- Internal Drives: Seagate IronWolf 3.5" NAS Drive (x1)
- Capacity: 8 TB total storage
- Serial Number: [omitted for privacy]
- Network: Connected via Ethernet to router
- Setup Environment: Configured on home network before deployment to church LAN

---

## 2. Initial NAS Setup

- Accessed DSM via find.synology.com
- Logged in to the DiskStation Manager (DSM) web interface
- Initialized storage pool and volume

---

## 3. Shared Folder Configuration

- Created shared folder: `ChurchCloud`
- Set folder permissions for project admin account
- Folder designated for cloud-accessible files and media

---

## 4. Synology Drive Setup

- Installed Synology Drive Server from Package Center
- Waited through initialization countdown

![Drive Initialization Countdown](images/Countdown.png)

- Enabled the `ChurchCloud` folder as a Team Folder in Synology Drive Admin Console

---

## 5. Access from Local Machines

### Windows
- File Explorer > Map Network Drive
- Path: `\\[NAS-IP]\ChurchCloud`

### macOS
- Finder > Go > Connect to Server
- Path: `smb://[NAS-IP]/ChurchCloud`

---

## 6. Deployment Considerations

- The NAS was initially configured on a home network
- Will be moved to the church’s internal LAN for production use
- IP address will change, so shared folder mappings will need to be updated
- System configuration and data will persist

---

## 7. Optional: Remote Access

- Enabled QuickConnect via Control Panel > External Access
- Provides remote access via Synology Drive apps and browser



