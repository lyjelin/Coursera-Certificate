Aug 10 2021

> 
- Technical support fundamentals
- The Bits and Bytes of Computer Networking
- Operating Systems and You: Becoming a Power User
- **System Administration and IT Infrastructure Services**
- IT Security: Defense against the digital dark arts


## System Administration and IT Infrastructure Services

### Week 1

IT infrastructure : encompasses the software, hardware, network, an services required for an organization to operate in an enterprise IT environment

System Administration : sysadmin is responsible for their company's I.T. 

Cloud computing : The concept that user can access user's data, use applications, store files from anywhere in the world as long as user has an internet connection

System Administration Task 
1. Decide what computer policies to user
2. Manage users and hardware
3. Responsible for user machine (i.e. printer)
4. Routine Maintenance 

	Hardware lifecycle
    1. Procurement
    2. Deployment
    3. Maintenance
    4. Retirement

### Week 2

Types of IT Infrastructure Services
- Physical
- Software
- Network
- Directory

> 
1. IaaS (Infrastructure as a Service)
IaaS provider give user pre-configured virtual machines that user can user just as if user had a physical server
2. NaaS (Network as a Service)
NaaS allows companies to offshore their networking services so that they don't have to deal with the expensive networking hardware
3. SaaS (Software as a Service)
4. PaaS (Platform as a Service)

Physical Infrastructure Systems
- Server Operating Systems : Regular operatinng systems that are optimized for server functionality
- Virtualization 
	- Dedicated Hardware : Better performance, 
    - Virtualized Instance : Most cost-effective, easier maintenance, reduces points of failure

Network Services
- File Transfer Protocol `FTP` -  legacy way to transfer files from one computer to another over the Internet; not secure due to no data encryption
	- Secured File Transfer Protocol `SFTP` - secured version of file transfer (SSH encryprion + Authentication)
	- Trivial File Transfer Protocol `TFTP` - 
- Network Time Protocol `NTP` - allow machines to synchronize their clocks (Ubuntu installations include a daemon that runs on the machine and is in charge of synchronizing the clock using NTP)
	- i.e. NTP daemon running status check in Linux `service NTP status`

### Week 3

> Software services
- Communication services (i.e. instant communication)
- Security services
- User productivity services
- File services
- Platform services
- Cloud recources

Email Services
1. POP3 - Good security, Good when have limited Quota, Can retrieve email
2. IMAP - Can retrieve email, Can receive email in multiple devices
3. SMTP - Can send & retreive email

File Services
- File storage services allow us to centrally store files and manage access between files and groups.
- Network File Storage : A protocol that enables files to be shared over a network
	- SAMBA : is a software service suite used for file services 
    - SMB : is a protocol that Samba implements
    - NAS : network attached storage, computers that are optimized for file storage
    
Platform Services
- Platform services provide a platform for developers to completely build and deploy software applications, without having to deal with OS maintenance, server hardware, networking or other services that are needed to use the platform tools
- i.e. apache
- Database server (i.e. MySQL, PostgreSQL)

Trouble shooting tools
- i.e. HTTP status code : codes or numbers that indicate some sort of error or info messages that occurred when trying to access a web resource
	- 4xx error : client side issue
    - 5xx error : server side issue
    - 2xx : successful

Cloud
- SaaS : software is already pre-configured and the user isn't deeply involved in the cloud configuration
- IaaS : user hosting your own services in the cloud
- Zone : locations where each of the data center are in
- Public/Private/Hybrid Cloud

















