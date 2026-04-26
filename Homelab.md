## Description
Lab Project with two Virtual Machines to implement and document networking, security and administration services. 


## Objetive
Learn and show abilities on Linux System Administration, Networking, Firewalls and SELinux.


## Machines
* A Bare Machine, in this case i used a server Dell PowerEdge R710 with Proxmox, but you can use any Laptop or PC with VirtualBox, VMware or KVM.
* A Virtual Machine with RHEL 9, or any distro based on the same, such as Rocky Linux 9, Alma Linux 9, etc. This will work as a Master Server with all the services.
* A Virtual Machine with Windows Server 10. This will work as a Client Test (SSH, Browser, FTP, etc.).
* A Virtual Machine with any BSD distribution. This will work as a Client Test (SSH, Browser, FTP, etc.).


## Project Order

* Installation
### Network
* Configure static network
* Hostname, DNS
* Reverse DNS

### Users, groups and repositories
* Create Groups (`admins`, `developers`)
* Create Physical Users with pass
*  Configure Sudo for admins group
* Repositories (`EPEL`, `BaseOS`, `AppStream` and `DNF`)

### FileSystems and Storage
* Add virtual disks
* Partitions (fdisk or gdisk) and formats (mkfs)
* LVM

### Main Services
* SystemD: Create a Deamon and explore 
* SSH: Configure to only allow users from `admins` group, change port, prove connection
* *Firewall (Nftables and Firewalld)* ______: Enable, add ssh and others services and open ports.
* *SELinux* ______: Activate `Enforcing` mode, verify ssh, etc.

### Network Services
* Apache and **SSL**: Create a simple page, open port 80 on firewall and test on windows.
* SQL (MariaDB): Create a bd, remote user (from windows).
* NFS: Share a directory and mount on the same VM (loopback) or another.

### Optional Services
* FTP (vsftpd)
* Samba *`
* Proxy
* Mail (Postfix + Dovecot)
* CUPS
* Docker or Podman
* Cockpit

Extra: Access rootless and Chroot
