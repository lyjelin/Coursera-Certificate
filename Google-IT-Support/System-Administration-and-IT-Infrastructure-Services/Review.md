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

### Week 4

> 
Directory services

- Directory Server : Contains a lookup service that provides mapping between network resources and their network addresses
- Replication : The stored directory data can be copied and distributed across a number of physically distributed servers but still appear as one unified data store for querying and administering
	- Replication is important because it provides redundancy by having multiple servers available simultaneously, so there will be minimal disruption to the service in the event that one of the server explodes
    - Replication also decreases latency when user access the directory service

Directory services : Userful for organizing data and making it searchable for an organization
- Implementing Directory Services : i.e. `Directory System Protocol` DSP, `Directosy Information Shadowing Protocol` DISP, `Directosy Operational Bindings Management Protocol` DOP, Lightweight Directory Access Protocol `LDAP` 

Centralized Management : A central service that provides instructions to all of the different parts of my IT infrastructure
- Directory services provide centralized `authentication`, `authorization`, and `accounting`, also known as AAA

LDAP 
- Used to access information in directory services like over a network
- **Active directory / OpenLDAP**
- LDAP entry; i.e. `dn:CN=Devan Sri-Tharan,OU=Sysadmin,DC=example,DC=com`
	- `dn` : distinguished name
    - `CN` : common name
    - `OU` : organizational unit
    - `DC` : domain component
- LDAP Authentication : (1) Anonymous (2) Simple (3) SASL

Active Directory `AD` : Native directory service for Microsoft Windows; AD also becomes the central repository of group policy machines `GPOs` which are ways to manage the configuration of Windows machines
- Active Directory Administrative Center `ADAC`
- Flexible Single-Master Operations `FSMO`
- Directory services are databases that are used to store information about objects 
- Group Policy : A set of policies and preferences that can be applied to a group of objects in the directory; A GPO can contain `computer configuration` (when computer starts), `user configuration` (when user logs on) or both

### Week 5

Data Recovery : process of trying to restore data after an unexpected event that results in data loss or corruption
- The best way to be prepared for a data-loss event is to have a well-thouht-out disaster plan and procedure in place
-  Disaster plans should involve making regular backups of any and all critical data that's necessary for your ongoing business processes.
- `Post-mortem` is a way for user to document any problems user discovered along the way, and most importantly, the ways user fixed them so user can make sure they don't happen again

Backing up Data
- i.e. Email databases, Sales Databases, Financial spreadsheets, Server configurations, Databases
- `Local storage` for backup :
	- Pros : Data is physically nearby, Low bandwidth needs
    - Cons : Data loss due to damage at location
- `Off-site storage` for backup :
	- Pros : Data is safer in multiple locations
    - Cons : Needs security and encryption, Needs large amounts of bandwidth
- Backup Solutions
	- `rsync` : File transfer utility that's designed to efficiently transfer and synchronize files between locations or computers.
- Testing Backups 
	- Restoration procedures : should be documented and accessible so that anyone with the right access can restore operations when needed
    - Disaster recovery testing : critical to ensuring a well functioning recovery system

Disaster recovery plan : A collection of documented procedures and plans on how to react and handle an emergency or disaster scenario, from the operational perspective
- Preventive measures : Any procedures or systems in place that will proactively minimize the impact of a disaster
- Detection measures : Meant to alert user and user's team that a disaster has occured that can be impact operations
- Corrective or recovery measures : Those enacted after a disaster has occured
- Designing a Disaster Recovery Plans : 
	1. Perform Risk Assessment : Allows person-in-charge to prioritize certain aspects of the organizations that are more at risk if there's an unforseen event
    2. Determine Backup and Recovery Systems
    3. Determine Detectopm & Alert Measures & Test Systems
    Determine Recovery measures
    
Post-mortem
- Sysadmins create a `post-mortem` after an incident, an outage, or some event when something goes wrong, or at the end of a project to analyze how it went
- Writing a Port-Mortem report : 
	1. Brief summary (dates, time, timezone)
    2. Detailed timeline (dates, time, timezone)
    3. Root cause (What can be learned?)
	4. Resoluctions and Recovery effects (dates, time, timezone)
    5. Actions to Avoid same scenario






















