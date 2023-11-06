# h1 - Install Debian on Virtualbox
HW: Lenovo ThinkPad T480
Host OS: Windows 11 PRO
Went: live amd64 folder on cdimage.debian.org
Used: debian-live-12.2.0-amd64-xfce.iso
Went: https://www.virtualbox.org/wiki/Downloads
Downloaded Windows Host virtual machine and tried to install it
Faced the problem and was requested to download frst Microsoft Visual C++ 2019
Went to Microsoft Visual studio page and downloaded Microsoft Visual C++ 2015- 2022 Redistributable (x64) 14.36.32532 as ARM64 failed
Tried again to install Windows Host virtual machine again
Instalation succedded 
Started VirtualBox. From the menus, select Machine: New...
"Create Virtual Machine", click "Expert Mode" to get all questions in one screen
Name: DebianTeroKarvinenCom
Type: Linux
Version: Debian (64-bit)
Memory Size: 4000 MB (more is better if you have enough RAM, 2000 MB could work)
Hard disk: Create a virtual hard disk now - yes <- did not see this option
Click "Finish"
Failed "Create Virtual Hard Disk", couldn't locate where this button is
Noticed that I can proceed to step "Insert Debian ISO Image as a Virtual CDROM" without previous step
Select your VM "DebianTeroKarvinenCom" and click "Settings".
Went "DebianTeroKarvinenCom - Settings", Storage tab
Under "Controller: IDE", choose the CDROM "Empty"
On the right, under "Attributes", beside "Optical Drive:" "IDE Secondary Master", click the tiny CDROM icon to open a menu
Choose Virtual Optical Disk File...
Find and select your ISO disk image (debian-live-12.2.0-amd64-xfce.iso)
Tried to start the virtual machine
Failed. Error message: VERR_FILE_NOT_FOUND
