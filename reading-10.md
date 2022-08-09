# Imaging, Backup, and Recovery

## Veem:

VeeamZIP – Creates an ad-hoc backup of a running VM, which gives you many benefits such as being able to easily copy a backup to another host without having to power off the original VM

Powerful and flexible restores – Supports a number of recovery scenarios, including recovery of an entire VM, guest OS files and individual application items

Quick Migration (VMware) – Migrates a live VM between hosts or datastores with minimal downtime and without requiring clusters, shared storage, or even VMware vMotion or Storage vMotion

VeeamZIP delivers technology that lets you create backups of running VMs. With VeeamZIP, you have to specify only two things – the VM you want to backup and where your resulting backup file will go. 

It’s that easy! The backup will be deduplicated (within the single VM being backed up) and compressed, resulting in significantly lower backup storage requirements. 

Many people ask what benefit this will provide in terms of disk space when only a single VM is involved, when I use VeeamZIP on a single VM; the disk savings are usually about half that of the VM’s actual usage on disk.  

The figure below shows a VeeamZIP ad-hoc backup being started:

You need to update a VM. Users frequently take a VeeamZIP backup before making any changes to a VM, such as before applying updates or patches.

You need to archive a VM. It’s simple to create a deduplicated and compressed copy of a VM before removing it from your virtual infrastructure.

You need to copy a VM to a remote host or test lab. VeeamZIP encapsulates VM configuration settings so you can easily transfer and run a VM in a different location.

VeeamZIP is also very efficient. The processing engine is fast, and optimizations include parallel processing of virtual disks, filtering out empty blocks, and more.
 
 
## Powerful and flexible restores

Veeam Backup Free Edition supports several data recovery scenarios, beginning with recovery of a VM file and going all the way to restoring an entire VM. 

The list includes:

Restoring VM files (.vmdk, .vmx and others for VMware; .vhd, .vhdx, .xml and others for Hyper-V). 
Veeam Backup Free restores VM files directly from deduplicated, compressed backups without having to extract the VM from the backup.

Restoring an entire VM. You can restore an entire VM to the same location or to a new location.

Restoring VM disks (VMware). If a VM disk becomes corrupted by an OS failure or some other cause, you can simply restore the affected VM disk and connect it to the original or recovered VM.

Restoring guest OS files. You can restore guest OS files for Windows FAT and NTFS file systems, and also ReFS with OS-level deduplication when running Windows Server 2012. Moreover, a special wizard and a virtual helper appliance provide support for 17 additional file systems. 

In all cases, Veeam Backup Free Edition is able to restore the guest files without having to extract the entire virtual disk image from the backup.

Quick Migration (VMware)

Quick Migration lets you migrate live VMs between hosts or datastores without requiring clusters, shared storage or advanced functionality that is not available in lower-level hypervisor editions. 

Quick Migration works well even in environments with slow or high latency connections that prevent VMware vMotion and Hyper-V Live Migration from working
 
## Additional v7 Features

1. Native tape support: Regardless of the fact that tapes are often considered an evil, they can be a necessary evil because many data centers continue to actively use them for archived or offsite backups. 
2. 
3. And this is understandable – tapes are portable, and long-term storage is inexpensive.

So, in v7, Veeam Backup Free Edition delivers one of features most frequently requested by users: native tape support. 

With this new capability, you can store individual files and VM backups on standalone tape drives and tape libraries (physical or virtual).

Additionally, native tape support is an excellent replacement for NTBackup, which was discontinued with the release of Windows Server 2003. 

Veeam Backup Free Edition even supports the format of tapes written by NTBackup, meaning you can use it to restore files from archives created by NTBackup!


2. Advanced support for VMware vCloud Director. v7 implements enhanced backup and recovery support for VMware vCloud Director (vCD). 

3. The metadata and attributes specific to vCD VMs are backed up, and you can restore VMs and vApps directly back to the original vCD location or to a new vCD location. 

4. And to ensure visibility, the vCD infrastructure is conveniently displayed in the management tree of the Veeam Backup Free Edition console.

5. Veeam Explorer for Microsoft SharePoint. Veeam Explorer for Microsoft SharePoint is a free tool built right into Veeam Backup Free Edition, making it easy for you to:

Search for individual items inside backups of SharePoint VMs

Recover items quickly and without agents

Send restored items as email attachments to specific users

Veeam Explorer for Microsoft SharePoint recovers items without pulling the whole VM image into production storage, which saves you premium storage space.  It also does not require installation of agents. 
 

