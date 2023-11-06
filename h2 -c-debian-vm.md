# h1 - Install Debian on Virtualbox
1. HW: Lenovo ThinkPad T480
2. Host OS: Windows 11 PRO
3. Went: live amd64 folder on cdimage.debian.org
4. Used: debian-live-12.2.0-amd64-xfce.iso
5. Went: https://www.virtualbox.org/wiki/Downloads
6. Downloaded Windows Host virtual machine and tried to install it
7. Faced the problem and was requested to download frst Microsoft Visual C++ 2019
8. Went to Microsoft Visual studio page and downloaded Microsoft Visual C++ 2015- 2022 Redistributable (x64) 14.36.32532 as ARM64 failed
9. Tried again to install Windows Host virtual machine again
10. Instalation succedded 
11. Started VirtualBox. From the menus, select Machine: New...
12. "Create Virtual Machine", click "Expert Mode" to get all questions in one screen
Name: DebianTeroKarvinenCom
Type: Linux
Version: Debian (64-bit)
Memory Size: 4000 MB (more is better if you have enough RAM, 2000 MB could work)
13. Hard disk: Create a virtual hard disk now - yes <- did not see this option
14. Click "Finish"
15. Failed "Create Virtual Hard Disk", couldn't locate where this button is
16. Noticed that I can proceed to step "Insert Debian ISO Image as a Virtual CDROM" without previous step
17. Select your VM "DebianTeroKarvinenCom" and click "Settings".
18. Went "DebianTeroKarvinenCom - Settings", Storage tab
19. Under "Controller: IDE", choose the CDROM "Empty"
20. On the right, under "Attributes", beside "Optical Drive:" "IDE Secondary Master", click the tiny CDROM icon to open a menu
21. Choose Virtual Optical Disk File...
22. Find and select your ISO disk image (debian-live-12.2.0-amd64-xfce.iso)
23. Tried to start the virtual machine
24. Failed. Error message: VERR_FILE_NOT_FOUND
