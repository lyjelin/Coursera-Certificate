# Operating Systems and You: Becoming a Power User

## Week 1

### Basic Commands

1. Using a Linux machine, you have the following directory tree:

```
/
|-- home
|   |-- cindy
|       |-- Pictures
|           |--Alaska
|           |--Canada
|       |-- Movies
|-- var
```

If your current path is /home/cindy/Pictures/Canada, and you want to change to the Alaska directory, which of the following commands can you use? Check all that apply.

- [x] **cd ~/Pictures/Alaska**
- [x] **cd ../Alaska**
- [ ] cd /Pictures/Alaska
- [x] **cd /home/cindy/Pictures/Alaska**

2. In Bash, which of the following commands can you use to view a long list of all files in the /home directory? Check all that apply.
- [ ] list -a /home
- [x] **ls -la /home**
- [x] **ls -l -a /home**
- [ ] ls -la ~

3. In Bash, which of the following commands can you use to remove a directory named: "Miscellaneous Directory?"
- [ ] rm Miscellaneous Directory
- [ ] rm -r Miscellaneous Directory
- [ ] rm Miscellaneous\ Directory
- [x] **rm -r Miscellaneous\ Directory**

### File and Text Manipulation

1. In Bash, which of the following commands can you use to view the contents of a document. Check all that apply. 
- [ ] open
- [x] **cat**
- [x] **less**
- [ ] dog

2. In a Linux machine, you have the following files: 

- apple.txt
- banana.jpg 
- chocolate.txt
- orange.txt

What command can you use to search for the word "fruit" in the text files in the above directory? Check all that apply.
- [x] **grep fruit apple.txt chocolate.txt orange.txt**
- [x] **grep fruit *.txt**
- [ ] find fruit apple.txt chocolate.txt
- [ ] find fruit apple.txt chocolate.txt orange.txt

3. In a Linux machine, you have a file named "types_of_fish.txt" and you want to append the word "trout" to the file contents. Which of the following commands can you use?
- [ ] echo trout < types_of_fish.txt
- [ ] echo trout > types_of_fish.txt
- [x] **echo trout >> types_of_fish.txt**
- [ ] echo trout 2> types_of_fish.txt

4. In a Linux machine, you want to list through a directory called /home/ben/Documents and search for the word "important" in the filenames in that directory. Which of the following commands can you use? 
- [x] **ls /home/ben/Documents | grep important**
- [ ] ls /home/ben/Documents >> grep important
- [ ] ls /home/ben/Documents < grep important
- [ ] ls /home/ben/Documents > grep important


## Week 3

### Software Disribution

1. What's the difference between an EXE file and an MSI file? Check all that apply
- [ ] An MSI file is an executable that can give you complete control over how your application should be installed
- [x] **An EXE file is an executable that may have an MSI file as one its resources**
- [x] **MSI files are used by the Windows Installer to control how your application is installed**


2. When would you want to use an MSI file to guide the installation of a program, as opposed to an EXE?
- [ ] When you want to be able to install your application on Linux as well as Windows
- [x] **When you want the Windows Installer to perform bookkeeping and setup for your application, at the cost of following the rules the Installer requires**
- [ ] When you want complete, custom control over how the application is installed

3. If you're performing an installation from the command line in Windows, what's the best method of checking out the options that the installation package provides? Check all that apply.
- [x] **Consult the documentation for the application to see what options they provide**
- [ ] Decide you don't want to install the application from the command line and use the GUI instead
- [x] **Try to use the /?, /h, or /help flags when running the package to see if they provide any helpful output**

4. What's the difference between apt and dpkg? Check all that apply.
- [ ] dpkg installs package dependencies
- [x] **apt is used as a package manager**
- [x] **apt installs package dependencies**
- [x] **dpkg is used as a standalone Debian package command**

5. Which of the following file extensions are considered archives in Windows? Check all that apply.
- [x] **.tar**
- [ ] .exe
- [x] **.zip**
- [x] **.rar**

6. What's the PowerShell commandlet you can use to extract and compress archives right from the commandline? 
- [x] **Compress-Archive**
- [ ] tar
- [ ] 7zip

7. What's the purpose of a DLL in Windows?
- [ ] To take up space on your hard drive
- [ ] To guid the installation of a package wia the Windows installer
- [x] **To share a pacakge of useful code among programs**

8. Most shared libraries in Windows are managed by which of the following?
- [ ] Left-and-right appendages, or LRAs
- [ ] Dynamic Linked Libraries, or DLLs
- [x] **Side-by-side assemblies, or SxS**

9. What's the correct commandlet to use in order to find a software package in the available package sources from the PowerShell command line?
- [ ] Get-PackageSource
- [ ] Register-PackageSource
- [x] **Find-Pacakage**

### Package Managers

1. Which of the following PowerShell commands will install the package "awesomesoftware" from the Chocolatey software source?
- [x] **Install-Package -Name awesomesoftware -Source chocolatey**
- [ ] Install-Package -Name chocolatey -Source awesomesoftware 
- [ ] Install-Package -Name awesomesoftware -Source MicrosoftWindows

2. Before you install software, which of the following commands should you run to get an updated version of your software?
- [ ] apt install
- [x] **apt update**
- [ ] apt remove
- [ ] apt search

### What’s happening in the background?

1. Which of the following tools allows you to create or edit MSI files?
- [ ] Process monitor
- [x] **Orca**
- [ ] Setup.exe

### Device Software Management

1. Which of the following is the piece of information that Windows will use to search for the right driver for a new piece of hardware connected to a Windows computer?
- [ ] PnP code
- [x] **Hardware ID**
- [ ] Drive Identification Number, or DiD

2. In Linux, in the /dev directory, devices that start with sd can be associated with what type of device? Check all that apply.
- [ ] Speakers
- [x] **Hard drives**
- [x] **USB drives**
- [x] **Memory sticks**

3. Which of the following correctly describes a "Security Patch?" 
- [x] **A piece of software that's meant to fix up a security hole.**
- [ ] A piece of fabric that's meant to patch a broken cable.
- [ ] An entirely new, more secure, version of an operating system.

## Week 4

### Filesystem Types

1. Which of the following is a characteristic of the FAT32 filesystem? Check all that apply.
- [x] **It doesn't support files larger than 4GB.**
- [x] **It's read and write compatible with Windows, Mac, and Linux OSes.**
- [x] **Its filesystem size can't be larger than 32GB.**
- [ ] It supports files up to 8GB in size.

2. What's the difference between a GPT and MBR partition table? Check all that apply.
- [x] **MBR only allows you to have volume sizes of 2TBs or less.**
- [ ] MBR is the new standard for partition tables.
- [x] **GPT doesn't have a limit to the amount of partitions you can make.**
- [x] **GPT allows you to have volume sizes of 2TBs or greater.**

3. Before you can store files on a hard drive, which of the following has to be done? Check all that apply.
- [ ] Nothing; hard drives can be used to store files out of the box
- [x] **Format a filesystem**
- [x] **Partition the disk**
- [x] **Mount the filesystem**

4. You want to format a partition with NTFS, and know that the data you'll be storing will consist mostly of many small files. In order to use as little space as possible, should you choose a larger or smaller Allocation Unit Size during the formatting process?
- [ ] Larger allocation unit size
- [X] **Smaller allocation unit size**

5. In Linux, what could a device named /dev/sdb2 refer to?
- [ ] The first hard drive that was detected on the system
- [x] **The second partition of the second hard drive detected on the system**
- [ ] The second B hard drive
- [ ] The first partition of the second hard drive detected on the system

6. True or false: If you want to save space on a Windows computer, deleting the pagefile.sys file is a good idea. 
- [ ] True
- [x] **False**

7. Which of the following commands in Windows will create a symbolic link called "cauliflower" to a file named "broccoli.txt?"
- [x] **mklink cauliflower broccoli.txt**
- [ ] mklink broccoli.txt cauliflower
- [ ] mklink /H cauliflower broccoli.txt

8. True or false: In modern versions of Windows, it's necessary to periodically run a Disk Defragmentation process manually to keep your disk healthy.
- [ ] True
- [x] **False**

9. In Linux, what's the difference between the commands df and du? Check all that apply
- [x] **df is used to find the amount of free space on an entire machine.**
- [x] **du is used to find the amount of disk usage on a specific directory.** 
- [ ] df is used to delete files in a directory.
- [ ] du is used to undelete files in a directory.

10. In Linux, what's the difference between a hardlink and a softlink? Check all that apply.
- [x] **A softlink points to a filename.**
- [x] **A hardlink points to an inode.**
- [ ] A hardlink points to a filename.
- [x] **You can view the hardlink count of a file using ls -l.**

11. Although NTFS is largely a self-healing filesystem, which of the following tools can you run to try to locate and repair serious disk corruption of the C: drive?
- [x] **chkdsk /r c:**
- [ ] chkdsk c:
- [ ] fsck c:

12. If you want to automatically mount a filesystem on computer startup, what file do you have to modify? 
- [x] **/etc/fstab**
- [ ] /dev/sda
- [ ] /etc/sudoers
- [ ] /etc/group

## Week 5

### Life of a Process

1. True or false: Windows processes can operate independently of their parents.
- [x] **True**
- [ ] False

### Managing Processes

1. Which of the following tools can help you gather information about the processes running on a Windows operating system?
- [ ] The Task Manager
- [ ] The tasklist utility from a command prompt
- [ ] The Get-Process commandlet from a PowerShell prompt
- [x] **All of the above**

2. If you restart a process using the Process Explorer utility, what will the new parent of that process be?
- [ ] cmd.exe
- [x] **Process Explorer**
- [ ] windows.exe
- [ ] momanddad.exe



