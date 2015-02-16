Title: Install VmWare Tools Ubuntu 
Author: David McQue
Date: 11/02/15


#Installing VMware Tools ubuntu 

Go to Virtual Machine > Install VMware Tools (or VM > Install VMware Tools).


1. In the guest, run :-

	Create a directory to mount the CD-ROM by running the command:

	`sudo mkdir /mnt/cdrom`

	When prompted for a password, enter your Ubuntu admin user password.


2. Mount the CD-ROM by running the command:

	`sudo mount /dev/sr0 /mnt/cdrom`


3. Extract the contents of the VMware Tools bundle by running the command:

	`tar xzvf /mnt/cdrom/VMwareTools-x.x.x-xxxx.tar.gz -C /tmp/`


4. Change directories into the VMware Tools distribution by running the command:

	`cd /tmp/vmware-tools-distrib/`

5. Install VMware Tools by running the command:

	`sudo ./vmware-install.pl -d`


6. Run this command to reboot the virtual machine after the installation completes:

	`sudo reboot now`

[For more info](http://kb.vmware.com/selfservice/microsites/search.do?language=en_US&cmd=displayKC&externalId=1022525)