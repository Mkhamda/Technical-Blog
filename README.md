#CIS 141 Technical Blog
#Michael Khamdalanikone
###mkhamdalanikone@gmail.com

#### Biography
My name is Michael Khamdalanikone and I am a CIS Networking and Security major at Sierra College. I also have an Associate's Degree in Natural Science. I currently work in Biology at a Laboratory that does pharmaceutical research. I hope to switch careers and one day become a Network Administrator. 

I live in Roseville, California with my wife and young Son. In my freetime I enjoy doing things outdoors and in the wilderness. I like the peacefulness that it affords and it really makes me feel connected to the world. It also makes me feel really small in the big picture but it is also humbling at the same time.

#### Skill 1.1 writing prompt.
At school, work or home, find a PC that has not yet been upgraded to Windows 10 (or role play with one that is upgraded to Windows 10).
Who is the primary user of the PC?
What are the technical specifications of that machine, as compared to the Windows 10 minimum requirements?
How would you go about upgrading this machine?  Why did you choose this approach?  Did you use any Microsoft tools to help determine your upgrade?  If so, which tools?
What version of Windows 10 would you install?  Why?

#### Skill 1.1 Response
   	I have an older laptop at home that used to run Windows, but currently runs Ubuntu. It is mostly a tinkering machine for me to try new distros on. It is a no frills laptop, but it's also pretty well equipped. The CPU is a i3-5020 @2.20 GHz with Intel graphics 5500. It also has 4gb of ram and a 1 TB HDD. The minimum requirements for WIndows 10 are    a 1 GHz processor, 1 GB of ram and 20 GB of storage on the HDD. This computer should be able to run Windows without a hitch. If I were to install WIndows 10 on this machine I believe I would do a clean install on an SSD. The storage component of the computer is currently where the bottleneck in performance would occur, and starting out fresh would allow me to preserve the current settings in case I need to revert back. I would install Windows 10 home because it is more affordable than Windows 10 pro and has most of the same features. I do not need the networking capability because this is a personal device for home and school use only. 



## Skill 1.1 - Prepare for Installation Requirements

####Warm up - How many computers are in V-129? I believe there are about 75 computers in V-129 at the moment.
There are 32 desktop computers in the room, but there are also personal laptops in the room. Also it is almost a
certainty that everyone has a smart phone in their pocket, which can be considered a personal computer.

####Not in class
Determine requirements for particular features such as Hyper V, Cortana, Miracast.
Configure upgrade readiness. distributed through Azure platform. Cloud readiness.

####In class
Determine hardware requirements and compatibility;
choose between an upgrade and a clean installation;
determine appropriate editions according to device type;
determine and create appropriate installation media;

Windows 10 supports many devices, including phones.
Editions: Windows 10 home, pro, enterprise, mobile, mobile enterprise, 10 IOT Core, Windows 10 S

Specs
Processor 1GHz or faster, RAM 1GB for 32-bit 2GB for 64-bit, Hard disk space 16 GB for 32-bit or 20 GB for 64-Bit
Graphics card: DirectX 9 or later with WDDM 1.0 driver, display 800x600

Deployment Options
Wipe and load        In-Place upgrade        Provisioning
viable for all        For existing windows 7/8/8.1    for windows 10 CYOD
scenarios                        scenarios

Different considerations for reasons to use different upgrade options.
Explore links that show the tools that Microsoft provides in order to test compatibility of Windows.

### Warm Up  Since We Last Met

####Task: Research a newsworthy event related to Windows 10, Microsoft, Cybersecurity and/or Information Technology. 

Microsoft has thwarted a Russian attack on two U.S. Agencies. It seized the websites of suspected Russian hackers who were supporting the Russian G.R.U. The two sites hacked were the Hudson Institute and the International Republican Institute. The hackers made fake web pages designed to look like the real web pages in order to steal login information of the people who used those sites. Russia has ramped up its attempts to break into Conservative Think Tanks recently. The two think tanks targeted have been critical of President Vladmir Putin. The attempted attacks are called spear-phishing, which is a highly targeted form of phishing. Phishing is when fake web pages or login pages are created in order to get people to input their login information. This can be stopped by multi-factor authentication and making sure to only click links that you know are trusted.These most recent attacks are thought to be aimed at attacking the U.S. midterm elections of 2018. 

Source: <https://www.nytimes.com/2018/08/21/us/politics/russia-cyber-hack.html>

## Your technical blogs
Hits- thorough, included prompt text, included notes from section. 
Misses- incomplete answers, Didn't Address Prompt, Spelling and punctuation. 

** Markdown 10 - available on the the Windows Store, has live preview of what you're typing as a web page. 
** Atom.io is another text editor that allows packages to be installed. 

####Snipping Tool

#Install Windows 10!
We will perform a clean install of Windows 10 Education.
Download disk image from class files
Using VMWare Workstation Player 14
Installing from ISO file
 
####Settings
+ 100GB of Storage on single disk
+ 4GB of RAM
+ 4 Cores
+ Everything else else left alone

## Steps
1. Create new Virtual Machine without Operating System Loaded( We will manually add it later) 
2. After Machine is loaded, we will load a Windows 10 installation â€œdiskâ€ onto the machine. If Computer will not boot, there could be a problem with the BIOS settings. Machine may be set to boot from network and therefore is waiting for a network connection. 
3. English as language and time format, You can add different languages and regions later.
4. You can install using the keyboard only if mouse drivers are not installed.
5. Input Software Key 8PHVN-VYCHH-QKM76-CQM93-C37Y9
6. Accept Agreements and continue

##Skill 1.2 
#####In what ways is the Media Creation Tool similar to the DIY USB installation?  In what ways is it different?
	It is similar in that it will create a bootable ISO file on the USB drive, but different in that it is mostly automated. If you plan on customizing the installation you will have to do the DIY media creation in order to insert the correct scripts into the installation files. 
#####Why would a user be interested in multiple partitions on a hard drive?  Use a Windows tool (GUI or CLI) to create a partition and describe the steps that you took to create multiple partitions.
	A user sometimes runs multiple operating systems from a single disk. In order to do this they will have to keep separate partitions on that disk with each operating system. They could also keep certain files on another disk altogether.
#####The GUI tool to partition the drive is diskmgmt.msc, The CLI tool to partition is called diskpart. 
#####Describe each step that requires "user attention" during the clean installation of Windows 10.
	There are very little parts of the Windows installation that require user attention anymore. The first is language and region, next is entering the software key. Finally after accepting all the documents there is another window about information collection and privacy. There you can choose what information is shared with microsoft and how they can use it. 
What is one Windows Feature that you chose to add after installation?  How did you add that feature?
    One feature that I added was Hyper-V, This was added through the OptionalWindowsFeatures.exe

### Warm-Up activity 9/17/2018
####What is â€œPatch Tuesdayâ€? When did it last occur? What was included in the most recent?

    Patch Tuesday is the day that Microsoft releases updates on a regular monthly schedule. It normally occurs on the second Tuesday of every month and sometimes on the fourth Tuesday if something went horribly wrong with the previous patch(it does, fairly often). The last one occured on September 11, 2018. It covered 61 vulnerabilities 17 of which were deemed critical. Most of the updates included patches to remote code execution in Microsoft's core programs such as Internet Explorer, Microsoft Edge, Microsoft Office, and .NET Framework. The most critical code that was patched was a zero-day vulnerability that allowed people to run a program that would grant administrator privileges to whomever ran it.   A lot of Administrators will hold off on updates for a week or two because Microsoft is notorious for breaking some things when releasing their patches. 

### Skill 1.2 Blog continued 9/17/2018
#####On Windows 8.1, install an application that may not be Windows 10 compatible.  Why do you think this application may not be compatible?
	I installed a copy of Winrar which is a file zipping software and VLC media player. These two programs should still be compatible because they are 64-bit programs. In theory Windows does allow for older programs to run on new machines even if they will not run properly.
#####Create a very special text file that you would like to be included in the upgrade.  What is in the file?  Where is it located?
	The text file I created was just a simple hello world rich text file and I left it on the desktop to easily see if it will survive the upgrade process. 
#####Describe each step that requires "user attention" during the in-place upgrade of Windows 10.
	Some of the things that required user input during the in-place upgrade were choosing what to keep and what to delete, reviewing the end-user agreements again, and ensuring that you have administrator privileges. 
#####In what ways was the upgrade process similar to  the clean install process?  How did it differ?
	This upgrade process was actually slower than a clean install because the upgrade process took the time to scan the machine and check all the programs and files already installed and ensure that the upgrade could take place. 
#####Are there any additional folders that remain after the upgrade process is complete?  What are the contents of those folders?
	All the original files remained after the in place upgrade. Another folder that showed up was one called Windows.old. This folder is actually the previous version of the OS in case we want to downgrade back. If we want to keep WIndows 10 we can delete the folder to free up space. 

###Skill 1.3 Blog Prompt
#####Create a list of hardware that a user might have that require a driver installation.
	Some hardware that might require drivers are: mice, keyboards, cameras, USB thumb drives, microphones, printers, scanners, fax machines, network cards, graphics cards, and aftermarket PC fans that can be programmed. 
#####Locate a device from your list (for example, printer or external storage) and install it on Windows 10 (VM in class, machine at home, maybe the host machine in class?)
	I had an old USB thumb drive in my backpack. 
#####Locate the version of the driver and see if it is the most current version available (in the case of the printer, check the manufacturer website).
######If necessary update the device.
	Windows provided a generic driver that worked to read it.
#####Disable the device.  Does this affect Windows performance?  What happens when you disable other devices?  Try disabling your network card - how was that experience?
	I disabled the device and the thumb drive disappeared from the file explorer. Once I disabled the network card I lost network connection. 
#####Why would I disable updates over metered connections?  Capture a screenshot of the screen on which you disabled this feature.
	I would disable updates over a metered connection because updates can be very large and I may not have enough data to complete the upgrade or it would be too costly to download so much data. 
#####Perform a "rollback" of a driver update.  Note, you will need to access a different USB device if you have been working with a printer.

#####After installing a USB microphone, a system has extremely poor performance.  How would you check to see if the performance issues are related to the USB microphone?
	I would first check to see if performance improves by removing the device to confirm that the device is causing the issue. Then I would check drivers. If all else fails I will have to check the documentation to ensure that the device is compatible with Windows 10

### Warm Up September 24 2018
#####What do you think is the future of operating systems?
	I think businesses looking to cut cost within their IT department may look at operating systems as a service as a viable option and some may even move to it. But overall I do not believe the majority of businesses will make the switch. Many corporations use custom made software within their infrastructures built for certain versions of Windows. Software development for businesses running their own software is actually quite slow because the businesses often attempt to make as little changes as necessary. Windows XP is still ran on many legacy systems because it functions as intended. Microsoft will have a huge battle ahead of itself if it believes that operating systems as a service can be viable. 

##Skill 1.4 Technical Blog Prompt
####Using your textbook, ITPro.tv videos and notes, as well as Microsoft documentation, research one of the following post-installation activities, create a step-by-step guide, and test out your guide on your VM.
 
â€¢Configure and customize the user interface per device type
â€¢Configure accessibility options
â€¢Configure Cortana
â€¢Configure Microsoft Edge
â€¢Configure Microsoft Internet Explorer
â€¢Configure Hyper-V
â€¢Configure power settings
##Skill 1.4 Answer
#####How to disable Microsoft's Internet Explorer 11 Completely
1. Click Window button lower left panel
2. Type in control panel
3. Click on Programs and Features
4. Click on Programs and Features again at the top of window this time.
5. Select turn Windows Features on or off
6. Uncheck Internet Explorer 11
7. Confirm Choice 
8. Click OK

#####How to disable Microsoft Edge Browser
1. Open a Windows Explorer Window
2. Navigate to Local Disk :C
3. Navigate to Windows Folder 
4. Navigate to SystemApps Folder
5. Right click on Microsoft.MicrosoftEdge_8wekyb3d8bbwe
6. Rename the file by adding something to the end
7. Edge will now be disabled

#####How to uninstall Edge Browser
1. Open powershell
2. Type get-appxpackage *edge* press enter
3. Type remove-appxpackage but do not press enter
4. Copy the Package Full Name 
5. Edge will now be uninstalled.
 
###Warm-Up October 1, 2018
####What is â€œUACâ€? Why is it important? When did Microsoft introduce UAC? Is UAC on your Sierra host machine different than your VM? If so, how?

		UAC is a security feature in Microsoft Windows. It stands for User Account Control. It is Microsoft's way of controlling user account privileges and restricting access to untrusted programs to administrators only. It was introduced with Windows Vista. The user account privileges are the same on both machines surprisingly. To view User Account Controls you can open the control panel, then click on user accounts and you can view the user account controls and changed them if need be. 
		There is a feature when UAC is activated. The background will dim the background and stop all processes until a user clicks, if not the computer will not activate change. 
 
##Skill 1.5 Enterprise implementations 
LSDO- permissions
+ Default settings are always LOCAL
+ Site permissions can take precedence over local
+ Domain- many machines, with potentially many sites with specific permissions
+ Organizational Unit- a group of users, or devices
#####This is implemented through Group Policy
Centralized control for User Settings, Computer Settings, Control and Deployment of Applications, Control User Experience
Gpupdate /force or logoff

##GPEdit Challenge
######Block all Microsoft Accounts
- Windows Settings, local policies, security options. It will be listed under Accounts: Block Microsoft accounts
######Enforce a password length of 10 characters? 
- This can be found under Windows Settings,  Password policy, Minimum password length. 
######Disable Secure desktop in UAC?( not recommended) 
-  Can be found in: Security Settings\Local Policies\Security Options. To turn it off disable â€œUser Account Control: Switch to secure desktop when prompting for elevationâ€

### Warm-Up October 8 2018
What is a â€œsoftwareâ€ bug? Describe the â€œbugâ€ that is delaying the release of the 1809 update for Windows 10. 
A software bug is an error, flaw, failure or fault in a computer program or system that causes it to produce an incorrect or unexpected result, or to behave in unintended ways. Most bugs come from the design or code of the programs or systems themselves and are usually not maliciously inserted. The â€œbugâ€ that is sporadically affecting the 1809 update to Windows 10 is an issue that some users are reporting the loss of files after updating. In April, Microsoft also faced an issue with Blue Screens of Death, but that bug was fixed before the update was released to the public. The current issue is still unresolved and there is not a lot of information yet on to what the bug is. 
<https://www.theverge.com/2018/10/6/17944966/microsoft-windows-10-october-2018-update-documents-deleted-issues-windows-update-paused>

### Notes Assessment and Deployment Kit
Microsoft ADK installation. Download from Microsoft.com Different tools can be installed within the ADK itself.  A test provision can be created. That way different settings and options can be used to help with installation on other devices.  We installed the Configuration Designer which allows you to set provisions of what the settings will be on end-user devices. These settings can be preloaded so that the users will not have to set up their new devices on their own. Many options are available including setting up what networks will connect to. 

### Networking
We are previewing the networking features in Windows. Microsoft now has a new way of changing settings that are not within control panel. One feature I could not easily locate within the new â€œSettingsâ€ was the Internet Options. It would appear when I searched it, but was not actually within the Networking and Internet tab. The network properties cannot be changed. Advanced sharing settings is where the public and private network types will live. This is where you can choose how you will share your personal information with other computers depending on your network. The Windows settings program is actually mostly hyperlinks. 
 We also watched a video about IPv4 and IPv6 addresses and Domain Name Servers. These are the core things needed for the internet to work. 
Network Reset can be used to help solve some network connectivity issues. It will remove and reinstall the network interfaces and reset all the settings. 
Wifi settings
Windows 10 now has an icon on the taskbar that will easily let you switch between wireless networks. You can connect and disconnect networks, manage which networks you will connect to. There is also an option to manage known networks. Here you can remove networks that you have connected to before so that you will NOT automatically connect when you are within range of the network. 
There is a new Windows feature that will obfuscate your MAC address. 
You can also add a VPN, Wifi Direct, or mobile hotspots to your device.

### Skill 2.1 Blog Prompt
Create a "Top 5" list of Windows 10 networking best practices, tips, tricks and troubleshooting strategies.
	Your list should include:
		1. An ordered list in markdown for each of the five items.
		2. A description for each item. What is the best practice, tip, trick or troubleshooting strategy?  How does this affect the end user?
		3. A hyperlink to online Microsoft document relating to each best practice, tip, trick or troubleshooting strategy.

### Skill 2.1 Answer
1. You can use a random MAC address when connecting to wireless networks to make it harder for people to track you. To enable this use the settings application and simply click use random hardware address.
<https://support.microsoft.com/en-us/help/4027925/windows-how-and-why-to-use-random-hardware-addresses>
2. You can reset all network settings if you are having trouble with connection issues with one click. Just go to the bottome of the network settings page and click reset to start fresh.
3. If you are having trouble conecting to a new wireless network, a restart should fix the problem. It is documented here:
<https://support.microsoft.com/en-us/help/3114149/windows-10-wireless-connection-displays-limited-status>
4. You can use metetered connections to limit automatic updates downloading in order to save data. 
<https://support.microsoft.com/en-us/help/4028458/windows-metered-connections-in-windows-10>
5. Windows 10 now easily allows you to figure out the wireless network's password if you are already connected. If you go to the network's setting and click security, you can figure out what the password is.
<https://support.microsoft.com/en-us/help/4023501/windows-find-wireless-network-password> 


### Warm-up Activity
What is Bitlocker? HOw is it configured? I have a USB drive that is configured with BitLocker. Will it work on all Windows 10 machines? How about a Macbook or a Chromebook?

Bitlocker is a full disk encryption feature included with Windows Professional or higher   Products. It does work on Mac with some tweak tools installed. BitLocker does not work on Chromebooks at all at the moment. BitLocker works along with your computer's TPM chip to create and hold the encryption keys. If you do not have a TPM chip enabled, you can still set it up, but you will need to use a USB flash drive to serve as the locker for the encryption keys. 

### MSCA Quiz Answers
Driver rollback question. You should rollback the printer driver. 
Internet Explorer question. Protected Mode, It now functions completely normal.
Power Consumption setting question. This is a custom setting. 

### Skill 2.2 Smackdown
Group 1 FAT file systems. Group 2 NTFS
Group 3 Stripped vs Group 3 Mirrored
Group 5 RAID General vs Group 6 Storage Spaces 

### Skill 2.2 Blog Prompt
In your technical Blog, address the following two scenarios:
Scenario 1: Creating a Large Volume
You have a new desktop running Windows 10. However, you try to copy your file repository and find out that you do not have enough disk space. You have 400 GB of free disk space on your C drive and you have 3 smaller 500 GB drives. What can you do?

Scenario 2: Configuring a Storage Space/ Storage Pool
       You create a new storage pool for the following disks on your Windows 10 computer:
Serial ATA (SATA): 1 TB
Serial Attached SCSI (SAS): 1 TB
           SATA and SAS are two different types of drives with different connectors/interfaces.
           What is the maximum size you can allocate for your new storage space?
           
### Skill 2.2 Blog Answer
Scenario 1: You can set up a RAID system for your hard drives, but the larger drive will now be restricted to 500 GB. This is not ideal, but do have 4 drives available so you will have 2 TB available once RAID is set up. 
Scenario 2: You should still be able to set up a 2TB Storage Space. Even though the two drives are different, They are the same size, you should have no size standardization. 

### Skill 2.3 Answers
Lab9
Question 1.
3 printers are installed on this computer.
Q2. 
4 printers are now installed on this computer.
Q3. 
The printed file now has the extension of “.pm”
Q3.1 
The printed file now has a header that says this is a printed file at the top and a page number at the bottom
Q4. 
The Microsoft Print to PDF printer comes the default printer when the virtual printer is uninstalled.

Lab10
Q1.
There are 3 devices and 3 printers on this machine.
Q2.
There are now 4 printing devices on this computer.
Q3.
There is now an icon that shows that the printer is shared in the description at the bottom of the page.
Q4.
There are 3 printing devices on the PC1 computer.
Q5. 
There are now 4 printers on the PC1 computer
Q6.
The window that opens is called “Save Output as”
Q7.
The file appeared on the PC2 desktop because that was where the “printer” is.

Lab12
Q1. 
A standard user account was created in the account page. A person would sometimes want to change the user to an administrator account to allow more control over the computer. Administrators can have control and access to all files on a computer and make critical changes.
Q2.
The created shared directory called “SharedData” is shared with the student account.
Q3.
The three accounts that the directory can be shared with are student, TEST, and everyone.
Q4.
The two accounts the directory are now shared with are student and TEST.
Q5.
An access denied window appears when we try to alter the shared document because we only have read privledges.  


### Warm Up October 29 2018
Browse the Windows Store for an App that you find interesting. What app did you find that surpirsed you? Is there an essential app to your life missing that from the store? What is it and where can one find it?

The app that I found interesting is one called Cyberduck, it cost $23.99. The application is a Browser or GUI that helps with FTP, SFTP, WebDAV, S3, BackBlaze B2, and OpenStack Swift. It is essentially a GUI application that makes file transfers from the cloud to personal computers easier. I guess this would be helpful for people who already have files stored on the cloud. The application seemed weird to me because people who use Cloud Services or have FTP servers facing the web would already know how to use the commmand line. 

### File Sharing Activity
https://docs.google.com/presentation/d/1RurCYpIdaC7PLGcsi8ahw1N9ezsBEGQkmXFf8KLccKs/edit?usp=sharing

### Night of Case Studies
You work for a small business of 25 employees, split between two offices that are in different buildings but share a parking lot. 
You have been tasked with designing a file sharing solution that is fast, reliable, easy to use, and secure( yep, the Holy Grail).
What would you do?

Set up a Onedrive or SharePoint for the company. That way all users can share and collaborate easily. This setup does not require use to set up a server and requires little training for the users. If we were to set up a secure server and ran a VPN between the buildings it would require greater capital costs. 

### Skill 2.4 Blog Prompt
You work for a small business of 25 employees. Split between two offices that are in different buildings, but share a parking lot.
You have been tasked with deploying Microsoft Office to all machines, Adobe CS Suite to the Accounting team, and QuickBooks to the Accounting Team. You also want to allow users to selectively install Adobe Acrobat.

What would you do?

### Skill 2.4 Answser
Use MDT to create separate deployments when installing window. This way we can control what applications come pre-installed for each type of employee, if the department expands it will be easier to get the new user set up. Another way we could push applications to the employees is to use Group Policy. We can separate the different departments into different groups and push applications to them 


### Lab7 Remote Desktop Answers
1. The remote computer does not have remote desktop turned on currently
2. At the center top of the screen there is a blue bar that indicates which IP I am currently connected to remotely. 
3. The only power option available is the ability to disconnect.
4. It was necessary to log into the machine again because while remote desktop was in use, the computer was unavailable.
5. The file created by PC2 is located on the desktop.
6. Some benefits of using remote desktop are: The ability to troubleshoot for someone while not physically present, and the ability to access your computer when you are away from home. There is also the ability for the network administrator to administer and check on every machine remotely to confirm things are as they should be or that the computer is functioning properly.

### Skill 2.5 Technical Prompt
1. Joe is a new IT Director who is tasked with making sure his Windows 10 computer users can be assisted remotely. On his first day at the company, Joe was told that the Remote Assistance feature was not working for users after a new firewall was installed. What could be causing the problem and how should it be addressed?

A. The firewall most likely disabled all remote connections. This is because normal users do not need the ability or have all the skills to safely deploy remote connections. Joe can change the firewall settings to allow secure remote connections, or to only allow certain people to use remote connections. 

2. You are an administrator at the Contoso Corporation. You have a 12-person help desk that supports about 10,000 users spread out over a 5-building campus. You don’t have enough people to provide support staff visits to a user who is having problems. Describe the actions you can take to support your company users.

A. We can have the user enable remote connections, ask him what his issue is, and through remote desktop we could either fix the problem or let him know how to fix it. If the problem persists we can th


