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


