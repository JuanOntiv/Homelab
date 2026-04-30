# Homelab Server

> Linux system administration la project implementing networking, security and server services from sratch on bare metal using Alma Linux 9. 

---

## Overview

This project documents the setup and configuration of a home lab environment running on a Dell PowerEdge R710 with Proxmox as the hypervisor.
Includes configurations, notes, commands, and project decisions documented for learning, reference, and portfolio purposes.
 
---
 
## Environment
 
| Component | Details |
|-----------|---------|
| Hardware | Dell PowerEdge R710 |
| Hypervisor | Proxmox VE |
| Master Server OS | AlmaLinux 9 (Minimal Install) |
| Client 1 | Windows Server |
| Client 2 | BSD (TBD) |
| Master Server IP | 192.168.1.120/24 |
| Network | Bridge mode, static IPs |

---

## Project Roadmap

- [x] Installation
- [ ] Network Configuration
- [ ] Users, Groups & Repositories
- [ ] Filesystems & Storage (LVM)
- [ ] Main Services (SystemD, SSH, Firewall, SELinux)
- [ ] Network Services (Apache, MariaDB, NFS)
- [ ] Optional Services
- [ ] Automation

---

## Documentation Index
 
| # | Topic | Doc |
|---|-------|-----|
| 01 | Installation | [docs/01-installation.md](docs/01-installation.md) |
| 02 | Network Configuration | [docs/02-network.md](docs/02-network.md) |
| 03 | Users, Groups & Repos | [docs/03-users-groups.md](docs/03-users-groups.md) |
| 04 | Filesystems & LVM | [docs/04-storage.md](docs/04-storage.md) |
| 05 | SystemD | [docs/05-systemd.md](docs/05-systemd.md) |
| 06 | SSH | [docs/06-ssh.md](docs/06-ssh.md) |
| 07 | Firewall (Firewalld + Nftables) | [docs/07-firewall.md](docs/07-firewall.md) |
| 08 | SELinux | [docs/08-selinux.md](docs/08-selinux.md) |
| 09 | Apache & SSL | [docs/09-apache.md](docs/09-apache.md) |
| 10 | MariaDB | [docs/10-mariadb.md](docs/10-mariadb.md) |
| 11 | NFS | [docs/11-nfs.md](docs/11-nfs.md) |
 
