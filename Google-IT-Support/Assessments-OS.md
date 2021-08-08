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

