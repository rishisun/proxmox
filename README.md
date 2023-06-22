# COMMANDS related to ovirt and proxmox.


Migrating the OVIRT vms.

track down the VM disk on the ovirt cluster.
let assume the disk as hdp-en00
 
Copy the files to the proxmox cluster on the folder with enough space.

Create a VM (assume VM ID = 101 ) with no disk attached.

## Upload the to the disk to the VM with the below command. 

qm importdisk 101 hdp-en00 local-lvm

Here the local-lvm is the disk storage space for VM's and containers on the proxmix cluster.

