Aug 3 2021

> 
- Technical support fundamentals
- The Bits and Bytes of Computer Networking
- **Operating Systems and You: Becoming a Power User**
- System Administration and IT Infrastructure Services
- IT Security: Defense against the digital dark arts


## Operating Systems and You: Becoming a Power User 

### Week 1

> 
1. Basic Operating System Naviagation
2. File and Text Manipulation

Command Line Interfaces `CLI`
- If we want to fee hidden files in directories : `ls -F` `ls -a`
- Help : `ls --help` `man ls`
- Know current directory : `pwd`
- Check on previous commands : `history`
- Copy files : `cp`
- Copy files with same file extension : `cp *.jpg path/where/you/want/to/save
- Copy directories : `cp -r DirName`
- Remove Directories : `rm -r DirName`
- Show first 10 lines of file : `head fileName.txt`
- Show last 10 lines of file : `tail fileName.txt`
- Search within file : `grep word_to_search fileName.txt
- Redirect error msg `ls/ dir/ fake_dir 2> error_output.text`

> [GNU Emacs Guide](https://www.gnu.org/software/emacs/tour/)


### Week 2

> 
1. Users and Group
2. Permissions

Standard user : user who's given restricted access to a machine
Administrator : user that has complete control over a machine
Windows domain : network of computers, users, files, etc that are added to a central database
root user : first user that gets automatically created when we install a Linux OS.

Windows : Fils/Dir permissions are assigned using Access Control Lists `ACLs`
- DCLs
- SCLs

SetUID : used to allow a file to be run as the owner of the file.
Sticky bit : allows the file to be modified by anyone, but only removed by the owner or root

### Week 3

> 
1. Packages
2. Package Manager
3. Device SW management

|   	|Windows   	|Linux/MacOS   	| 
|---	|----------	|--------------	|
|.exe   |Y   		|   			|  
|.msi   |Y   		|   			| 
|.deb   |   		|Y [dpkg]  		|
|.apt   |   		|Y 		 		|
|.dpkg  |   		|Y  	  		|

`.exe` (contains instruction for a computer to execue when they're run
- Contains `.msi` file (Microsoft install package) : Used to guide a program valled he Windows installer in the installation, maintenance, and removal of programs on the Windows OS
- Can be used as stand-alone file with no custome installers, with no msi files

Archives 
- Package archives are basically the core or source software files that are compressed into one file
- `7-zip` [reference](https://www.7-zip.org/download.html) 

Dynamic-link libraries `DLL`
Side by Side Assembly `SxS`
- Manifest tells Windows to load the appropriate library from the SxS folder
- SxS system supports access to multiple versions of the same shared library automatically
Sysinternal package

**Package managers** comes with the works to make package installation and removal easier, including installing package dependencies
- if user install a standalone package, user won't automatically install its dependencies.
- Advanced Package Tool `apt` : Package manager for the Ubuntu OS
	- APT package manager is used to extend the functionality of `dpkg`
    - Makes package installation easier (installs package dependencies for user, makes it easer to find packages that user can install, cleans up package which is not needed)
    - `sudo apt upgrade` : Before installing new software, it's good to run APT update to make sure user is getting the most up-to-date software in one's repositories.

Package repositories : Repositories are servers that act like a central storage location for packages.
- PPA `Personal Pacakage Archive` : Software respository for uploading source packages to be built and published as an apt repository by Launchpad
	- PPA software isn't as vetted as repositories user might find from reputable sources like Ubuntu
    - They can sometimes contain defective, or even malicious software

The Windows installer uses the information stored on the tables in the MSI database, to guide how the installation should be performed. 
- They'll know where files and application data should go, and any other things that should happen to successfully install the program. 
- The Windows installer will keep track of all the actions it takes and create a separate set of instructions to undo them. 
- This is how it lets users uninstall the program.

Driver : used to help HW devices interact with our OS
- `devmgmt.msc` - window
- `dev` - Linux
	1. Character devices : keyboard/mouse; transmit data character by character
    2. Block devices : USB, Hard drives, DBROMs; transfer blocks of data, a data block is a unit of data storage
- `sd` : massive data storage
- Not all kernal modules are drivers

OS Updates
1. Windows
	- Security patch : software that's meant to fix up a security hole
    - Windows Updata Client Service
2. Linux
	- `apt update` or `apt upgrade`
    - Kernal : just another package
    - `uname` : gives system information (`uname -r` : verify latest kernal version)

### Week 4

> 
1. Disk Partitioning
2. Formatting Filesystem


Disk Anatomy
- Storage disk can be divided into partitions
- Partition : Piece of disk that user can manage
- Partition Table : tells the OS how the disk is partitioned; (i) MBR `Master Boot Record` (ii) GPT `GUID Partition Table`

- Mounting : Making something accessible to the computer, like a filesystem or a hard disk
- Swap space : Dedicated area of the hard drive used for virtual memory

Files
- NTFS `Native File System` of window
- NTFS use MFT `Master File Table`; Every file on a volume has at least one entry in MFT
- Symbolic link 
- Soft link (`soft link >> File >> HDD`)
- Hard link (`hard link >> Inode >> Inode Table >> HDD`)
- In Linux, **Inode** stores everything about a file, except filename and file data

Data buffer : region of RAM that's used to temporarily store data while it's being moved around
Data Corruption : can be caused by system failure/software bugs (NTFS has some advanced features built in that can help minimize the danger of corruptions, as well as, try to recover when the file system get damaged)

### Week 5

> 
Processes

Session Manager Subsystem : First non-kernal user mode that starts when window boots up or start

View Processes (in Linux) : 
- `ps -x`
	- `PID` : process id
	- `TTY` : terminal associated wih the process
	- `STAT` : Process status
- `ps -ef` 
	- `UID` : user ID of the person whp launched the process
    - `PPID` : parent id
    - `C` : # of children processes
    - `STIME` : start time of the process
    - `TIME` : total CPU time that the process has taken up
    - `CMD` : name of the command the process is running

Signal : A way to tell a process that something's just happened
- `SIGINT` signal interrupt (window)
- `SIGTERM` termination signal (linux)

### Week 6

> 
1. Remote Access
2. Virtualization
3. Logging

Remote connection file transfer > `SCP` Secure Copy (Used in Linux to copy files between computers on a network)

Virtualization
- Virtual instance : single virtual machine (i.e. virtualBox)

`log` (i.e. `console.log`) : Logs tell the exact time that an event occurred, who caused the event, and more
- Logging : Act of creating log events
- Windows - **Event Viewer** / `eventvwr.msc`
- Linux - stored in `/var/log` dir (`/var/log/syslog` contains the most comprehensive information about user's system)

Imaging Software
- Imaging a machine, means to format a machine with an image of another machine. This includes everything, from the operating system to the settings.
- OS Deployment Methods
	- i.e. Disk cloning tool : makes a copy of entire disk and allow user to back up a current machine or set a new one
    	- disk-to-disk cloning : connect an external hard drive (i.e. SDD) to the machine you want to clone
        









