# h1 - h2 Crown Jewels and Bad Guys
## Task X Read and summarize: Intelligence-Driven Computer Network Defense, Informed by Analysis of Adversary Campaigns and
## Intrusion Kill Chains

Such tools as intrusion detection systems and anti-virus are inefficent for new class of threats: "Advanced Persistent Threat" (APT). Kill chain model can help to mitigate potential intrusions.

"Advanced Persistent Threat" (APT) is a new trend in the world of threats, where intrusion detection systems and anti-virus are inefficent as APT is a stealthy threat actors, typically a state or state-sponsored group, which gains unauthorized access to a computer network and remains undetected for an extended period. Accroding to Hutchins et al 2011, responses to APT intrusions require an evolution in analysis, process, and technology.

It's interesting to see how modern cyber kill chain is different with kill chain descirbed in publication made by United States Department of Defense Joint Staff publication where the stages were identified as follow: find,fix, track, target, engage, and assess (U.S. Department of Defense, 2007).

My own observation is it's interesting to read about similarities in cyber kill chain and Improvised Explosive Device (IED) attacks. I would never think there are any similarities between those 2 activities.

The effect of intelligence-driven CND is a more resilient security posture. APT actors, by their nature,
attempt intrusion after intrusion, adjusting their operations based on the success or failure of each
attempt. In a kill chain model, just one mitigation breaks the chain and thwarts the adversary, therefore
any repetition by the adversary is a liability that defenders must recognize and leverage

Cyber killchain originates from  U.S. military targeting doctrine defines the steps of this process as find, fix, track, target, engage, assess
(F2T2EA)

Reading Table 1: Courses of Action Matrix there is nothing that can destroy the  intrusion



## Task C Install Debian on Virtualbox
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
