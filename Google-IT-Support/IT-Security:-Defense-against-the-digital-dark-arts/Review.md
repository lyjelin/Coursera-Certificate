Aug 21 2021


- Technical support fundamentals
- The Bits and Bytes of Computer Networking
- Operating Systems and You: Becoming a Power User
- System Administration and IT Infrastructure Services
- **IT Security: Defense against the digital dark arts**

## IT Security: Defense against the digital dark arts

### Week 1

#### Malicious Software

The CIA Traid
- CIA refers to `confidentiality` `integrity` `availability`
- CIA Traid : Guiding model for designing information security policies in the workplace and for your own personal environments

Essential Security Terms
- Risk : The possibility of suffering a loss in the event of an attack on the system
- Vulnerability : A flaw in the system that could be exploited to compromise the system 
	- i.e. 0-day vulnerability : A vulnerability that is not known to the software developer or vendor, but is known to an attacker; A vulnerability that has already been exploited before the vulnerability has been disclosed
- Exploit : Software that is used to take advantage of a security bug or vulnerability
- Threat : The possibility of danger that could exploit a vulnerability (possible attackers)
- Hacker : Someone who attempts to break into or exploit a system
- Attack : An actual attempt at causing harm to a system

Malicious Software
- Malware : type of malicious software that can be used to obtain your sensitive information or delete or modify files
	- i.e. viruses, worms, adware, spyware, trojans, rootkits, backdoors, botnets

#### Network attacks

Network Attack
- DNS Cache Poisoning attack : A DNS Cache Poisoning attack works by tricking a DNS server into accepting a fake DNS record that will point you to a compromised DNS server. It then feeds you fake DNS addresses when you try to access legitimate websites. It can spread to other networks too.
- Man-in-the-Middle-Attack : An attack that places the attacker in the middle of two hosts that think they're communicating directly with each other. 
	- Another way that man-in-the-middle attack can be established is via `rogue access point attack` and `evil twin attack`
    	1. Rogue AP : access point that is installed on the network without the network administrator's knowledge
        2. Evil Twin :  The premise of an evil twin attack is for you to connect to a network that is identical to yours. This identical network is our networks evil twin and is controlled by our attacker. Once we connect to it, they will be able to monitor our traffic.

Denial-of-Service 
- `DoS` attack : An attack that tried to prevent access to a service for legitimate users by overwhelming the network or server
- Ping of Death or POD, is a pretty simple example of a DoS attack : works by sending a malformed ping (larger in size than what the internet protocol can handle) to a computer
- Ping flood : sends tons of ping packets to a system (sends `ICMP echo requests`)
- SYN flood : the server is being bombarded with the SYN packets; The server is sending back SYN-ACK packets but the attacker is not sending ack messages. This means that the connection stays open and is taking up the server's resources. 
- Distributed Denial-of-Service `DDoS` Attack : A DoS attack using multiple systems

#### Other Attacks

Client-side Attacks
- Injection attacks; i.e. (i) `Cross-site scripting` (XSS) attacks : A type of injection attack where the attacker can insert malicious code and **target the user** of the service (ii) `SQL injection attack` targets the entire website if the website is useing a SQL database

Password Attacks
- Utilize software like password-crackers that try and guess user's password
- Brute force attack : just continuously tries different combinations of characters and letters until it gets access
- Dictionary attack : it tries out words that are commonly used in passwords

Deceptive Attacks
- Social Engineering : Attack methos that relies heavily on interactions with humans instead of computers
- Phishing attack : Phishing usually occurs when a malicious email is sent to a victim disguised as something legitimate, i.e. Spear phishing, Spoofing, Baiting, Tailgating

### Week 2

#### Symmetric Encryption

Cryptography
- `Encryption` : act of taking a message, called plaintext, and applying an operation to it, called a cipher. So that you receive a garbled, unreadable message as the output, called ciphertext.
- `Decryption` : reverse process of encryption, taking the garbled output and transforming it back into the readable plain text
- Encryption algorithm : The underlying logic of process that's used to convert the plaintext into ciphertext
- Security through obscurity
- Cryptosystem : Collection of algorithms for key generation and encryption and decryption operations that comprise a cryptographic service should remain secure, even if everything about the system is known except for the key
- Frequency analysis : practice of studying the frequency with which letters appear in ciphertext
- Steganography : The practive of hiding information from observers, but not encoding it

Symmetric Cryptography
- Kerchhoff's principle : `Key` is the most important component of the cipher to keep secret
- Symmetric-key algorithm : Same key is used to encrypt and decrypt the message
- Substitution cipher : encryption mechanism that replaces parts of your plaintext with ciphertext
- Stream cipher : Takes a stream of input and encrypts the stream one character or one digit at a time, outputting one encrypted character or digit at a time (one-to-one relationship)
- Block ciper : The cipher takes data in, places it into a bucket or block of data that's a fixed size, then encodes that entire block as one unit

Symmetric Cryptography Algorithms
- Data Encryption Standards `DES`
	- DES was adopted as a federal standard for encrypting and securing government data
    - It is a symmetric block cipher that uses 64-bit key sizes and operates on blocks 64-bits in size; Though the key size is technically 64-bits in length, 8-bits are used only for parity checking, a simple form of error checking. This means that real world key length for DES is only 56-bits.
- Federal Information Processing Standard `FIPS` 
- Key Length : defines the max potential strength of the system
- Advanced Encryption Standard `AES`
	- Symmetric block cipher
    - Uses 128-bit blocks and supports key lengths of 128-bit, 192-bit, or 256-bit
    - Due to the large key size, brute-force attacks on AES are only theoretical right now, because the computing power required exceeds anything feasible today
- Important thing to keep in mind when considering various encryption algorithms is speed and ease of implementation
- `RC4` Rivest Cipher 4 : Symmetric Stream ciper that gained widespread adoption because of its simplicity and speed
	- supports key sized from 40-bits to 2048-bits

### Week 2

#### Symmetric Encryption

Cryptography
- `Encryption` : act of taking a message, called plaintext, and applying an operation to it, called a cipher. So that you receive a garbled, unreadable message as the output, called ciphertext.
- `Decryption` : reverse process of encryption, taking the garbled output and transforming it back into the readable plain text
- Encryption algorithm : The underlying logic of process that's used to convert the plaintext into ciphertext
- Security through obscurity
- Cryptosystem : Collection of algorithms for key generation and encryption and decryption operations that comprise a cryptographic service should remain secure, even if everything about the system is known except for the key
- Frequency analysis : practice of studying the frequency with which letters appear in ciphertext
- Steganography : The practive of hiding information from observers, but not encoding it

Symmetric Cryptography
- Kerchhoff's principle : `Key` is the most important component of the cipher to keep secret
- Symmetric-key algorithm : Same key is used to encrypt and decrypt the message
- Substitution cipher : encryption mechanism that replaces parts of your plaintext with ciphertext
- Stream cipher : Takes a stream of input and encrypts the stream one character or one digit at a time, outputting one encrypted character or digit at a time (one-to-one relationship)
- Block ciper : The cipher takes data in, places it into a bucket or block of data that's a fixed size, then encodes that entire block as one unit

Symmetric Cryptography Algorithms
- Data Encryption Standards `DES`
	- DES was adopted as a federal standard for encrypting and securing government data
    - It is a symmetric block cipher that uses 64-bit key sizes and operates on blocks 64-bits in size; Though the key size is technically 64-bits in length, 8-bits are used only for parity checking, a simple form of error checking. This means that real world key length for DES is only 56-bits.
- Federal Information Processing Standard `FIPS` 
- Key Length : defines the max potential strength of the system
- Advanced Encryption Standard `AES`
	- Symmetric block cipher
    - Uses 128-bit blocks and supports key lengths of 128-bit, 192-bit, or 256-bit
    - Due to the large key size, brute-force attacks on AES are only theoretical right now, because the computing power required exceeds anything feasible today
- Important thing to keep in mind when considering various encryption algorithms is speed and ease of implementation
- `RC4` Rivest Cipher 4 : Symmetric Stream ciper that gained widespread adoption because of its simplicity and speed
	- supports key sized from 40-bits to 2048-bits

#### Public Key or Asymmetric Encryption

Asymmetric Cryptography
- Different key is used to encrypt and decrypt
- Public key && Private Key
- Allow secure communication over an untrusted channel
- `MAC` : A MAC is a bit of information that allows authentication of a received message, ensuring that the message came from the alleged sender and not a third party masquerading as them
	- HMAC : Keyed-hash message authentication code
    - CMAC : Cipher-based message authentication codes
    - CBC-MAC : Cipher block chaning message authentication codes

Asymmetric Encryption Algorithms
- Digital Signiture Algorithm `DSA` : covers key generation process along with the signing and verifying data using the key pairs
- Diffie-Hellman (DH Key exchange algorithm)
- Elliptic curve cryptography `ECC` : A public-key encryption system that uses the algebraic structure of elliptic curves over finite fields to generate secure keys  
	- Elliptic curve is composed of a set of coordinates that fit in equation ($y^2 = x^3 + ax + b$), have horizontal symmetry
- Both DH and DSA have elliptic curve variants, referred to as ECDH and ECDSA

#### Hashing

Hashing
- A type of function or operation that takes in an arbitary data input and maps it to an output of fixed size, called a hash or digest 
- You feed in any amount of data into a hash function and the resulting output will always be the same size, but the output should be unique to the input, such that two different inputs should never yield the same output
- Hashing can also be used to **identify duplicate data sets in databases** or **archives to speed up searching of tables** or **to remove duplicate data to save space**
- Cryptographic hashing is distinctly different from encryption because cryptographic hash functions should be one directional
- The ideal cryptographic hash function should be deterministic, meaning that the same input calue should always return the same hash value; The function should be quick to compute and be efficient; It should be infeasible to reverse the function and recover the plain text from the hash digest
- `Hash collision` : Two different inputs mapping to the same output

Hashing Algorithms
- MD5 : operates on a 512 bit blocks and generates 128 bit hash digests
- SHA-1
	- part of the secure hash algorithm suite of functions
    - operates on a 512 bit blocks and generates 160 bit hash digests
    - used in popular protocols like TLS/SSL, PGP SSH, and IPsec
    - Also used in version control systems like `Git`, which uses hashes to identify revisions and ensure data integrity by detecting corruption or tampering
- SHA-1 and SHA-2 were required for use in some US government cases for protection of sensitive information
- `MIC` Message Integrity Check : Hash digest of the message in question -  MICs as protecting against accidental corruption or loss, but not protecting against tampering or malicious action
- A successful brute force attack, against even the most secure system imaginable, is a function of attacker time and resources
- Password salt : Additional randomized data that's added into the hashing function to generate a hash that's unique to the password and salt combination
	- If large salt is used, the computational and storage requirements to generate useful rainbow tables become almost unfeasible


#### Cryptographic Application

Public Key Infrastructure `PKI`
- PKI is a system that defines the creation, storage and distribution of digital certificates
- Digital certificate : file that proves that an entity owns a certain public key; certificate contains information about the `public key`, the entity it belongs to and a digital signature from another party that has verified this information
- The entity that's responsible for storing, issuing, and signing certificates is referred to as `CA`, or **Certificate Authority**
- `RA`, or Registration Authority, is responsible for verifying the identities of any entities requesting certificates to be signed and stored with the CA.
- A central repository is needed to securly store and index keys, and a certificate management system of some sort makes managing access to store certificates and issuance of certificates easier
- i.e. SSL/TLS server certificate, self-signed certificate, SSL/TLS client certificate, code signing certificate, Root certificate
- PKI is very much dependent on trust relationships between entities, and building a network or chain of trust -> This chain of trust starts from the root certificate authority
- A certificate that has no authority as a CA is referred to an end-entity or leaf certificate
- `X.509` standars is what defines the format of digital certificates  (defines `version` `serial number` `certificate signiture algorithm` `issuer name` `validity` `subject` `subject public key info` `certificate signiture algorithm` `certificate signiture value`

Cryptography in Action
- `HTTPS` 
	- Secure version of HTTP
    - Essentially encapsulating the HTTP traffic over an encrypted, secured channel utilizing SSL or TLS.
- TLS is actually **independent of HTTPS**, and is actually a generic protocol to permit secure communications and authentication over a network; Also used to secure other communications aside from web browsing, like VoIP calls such as Skype or Hangouts, email, instant messaging, and even Wi-Fi network security
	1. A secure communication line, which means data being transmitted is protected from potential eavesdroppers
    2. The ability to authenticate both parties communicating, through typically only the server is authenticated by the client
    3. The integrity of communications, meaning there are checks to ensure that messages aren't lost or altered in transit
- TLS handshake
- Session key : Shared symmetric encryption key used in TLS sessions to encrypt data being sent back and forth
- Pretty Good Privacy `PGP` : An encryption application that allows authenticatio of data, along with privacy from third partied, relying upon asymmetric encryption to achieve this

Securing Network Traffic 
- VPN : sort of encrypted tunnel where all of user's remote system's network traffic would flow, transparently channeling the packets via the tunnel through the remote private network && Can be point-to-point
- `IPsec` Internet Protocol Security : VPN protocol designed in conjunction with IPv6
	- IPsec work by encrypting an IP packet and encapsulating the encrypted packet inside an IPsec packet.
    - IPsec supports 2 modes of operations
    	1. transpsernt mode : Only payload of the IP packet is encrypted, leaving IP headers untouched
        2. tunnel mode : The entire IP packet, header payload and all, is encrypted and encapsulated inside a new IP packet with new headers
- `L2TP` Layer 2 Tunneling Protocol : used to support VPN when data confidentiality is needed
- Secure communication is established using `Encapsulating Security Payload`
- Tunnel is provided by L2TP which permits the passing of unmodified packets from one network to another. Secure channel is provided by IPsec, which provides confidentiality, integrity, and authentication
- OpenVPN, OpenSSL

Cryptographic Hardware
- Trusted Platform Module `TPM` : Hardware device that's typically integrated into the hardware of a computer, that's a dedicated crypto processor
- TPM offers 
	1. secure generation of keys
    2. random number generation
    3. reomte attestation : Remote attestation is the idea of a system authenticating its software and hardware configuration to a remote system -> This enables the remote system to determine the integrity of the remote system
    4. data binding and sealing
- TPM has unique secret RSA key burned into the hardware at the time of manufacture, which allows a TPM to perform things like hardware authentication
- Full Disk Encryption

### Week 3

#### Authentication 

Authentication Best Practices
- Identification : Idea of sescribing an entity uniquely
- Authentication `authn` : Proving you who claim to be
- Security as Risk mitigation; It's impossible to complemetely eliminate the risk
- Incorporating good password policies into an organization is key to ensuring that employees are securing their accounts with strong passwords

Multifactor authentication
-  A system where users are authenticated by presenting multiple pieces of information or objects
	1. something you know
    2. something you have
    3. something you are
- Physical token (i.e. OTP `One-Time Password`)

Certificate 
- Certificates are public keys that are signed by a certificate authority or CA as a sign of trust
- In order to issue client certificates, an organization must setup and maintain CA infrastructure to issue and sign certificates
- Part of certificate authentication also involves the client authenticating the server, giving us mutual authentication

LDAP
- `Lightweight Directory Access Protocol` is an open industry-standard protocol for accessing and maintaining directory services
- DAP specification describes the data structure of the directory itself and defines functions for interacting with the service, like performing look ups and modifying data
- The structure of an LDAP directory is a sort of tree layout and is optimized for retrieval of data more so than writing.
- Directories can be hosted across lots of different LDAP servers to facilitate more rapid look ups, and are kept in sync through replication of the directory
- LDAP uses a tree structure called a Data Information Tree, objects will have one parent and can have one or more children that belong to the parent object

Remote Authentication Dial-In User Service `RADIUS`
- Protocol that provides AAA services for users on a network
- Used to manage access to internal networks, WiFi networks, email services and VPN services.
- Originally designed to transport authentication information for remote dial up users, It's evolved to carry a wide variety of standard authentication protocols like EAP or Extensible Authentication Protocol

Kerberos
- Network authentication protocol that uses tickets to allow entities to prove their identity over potentially insecure channels to provide mutual authentication
- It also uses symmetric encryption to protect protocol messages from eavesdropping and replay attacks

TACACS+ `Terminal Access controller Access-Control System Plus`
- It's a Cisco developed AAA protocol
- **TACACS+ is primarily used for device administration, authentication, authorization, and accounting, as opposed to RADIUS, which is mostly used for network access AAA**

Single Sign-On
- Authentication concept that allows users to authenticate once to be granted access to a lot of different services and applications
- SSO is accomplished by authenticating to a central authentication server, like an LDAP server -> This then provides a cookie, or token that can be used to get access to applications configured to use SSO
- i.e. of SSO system is the openID, the centralized authentication system

#### Authorization

Authorization and Access Control Methods
- `Authorization` pertains to describing what the user account has access to or doesn't have access to

Access Control
- `OAuth` : An open standard that allows users to grant third-party websites and applications access to their information without sharing account credentials.
	- This can be thought of as a form of access delegation because access to the user's account is being delegated to the third party.
    - This is accomplished by prompting the user to confirm that they agree to permit the third party access to certain information about their account
- It's important that users pay attention to what third party is requesting access and what exactly they're granting access to. 
- **OAuth permissions can be used in phishing style attacks to gain access to accounts without requiring credentials to be compromised** -> This works by sending phishing emails to potential victims that look like legitimate OAuth authorization requests, which ask the user to grant access to some aspects of their account through OAuth.

Access Control List `ACL`
- A way of defining permissions or authorizations for objects
- A file system would have an ACL, which is a table or database with a list of entries specifying access rights for individuals or groups for various objects on the file system like folders, files or programs. -> `These individual access permissions per object are called Access Control Entries and they make up the ACL`
- ACLs are also used extensively in network security, applying access controls to routers switches and firewalls
- Network ACLs are used for restricting and controlling access to hoster services running on hosts within your network
- Network ACLs can be defined for incoming and outgoing traffic.
- Network ACLs can also be used to restrict external access to systems and limit outgoing traffic to enforce policies or to prevent unauthorized outbound data transfers.

#### Accounting

Tracking Usage and Access
- Accounting : Keeping records of what resources and services your users access or what they did when they were using your systems
	- Critical component of this is a`uditing`, which involves reviewing these records to ensure that nothing is out of the ordinary

### Week 4

#### Secure Network Architecture

Network Hardening Best Practices
- Network Hardening : Processof securing a network by reducing its potential vulnerabilities through configuration changes and taking specific steps
- General security principle : concept of disabling unnecessary extra services or restricting access to them
- Implicit deny : Network security concept where anything not explicitly permitted or allowed should be denied
- Important : **Monitoring & Analyzing traffic of network**
- `Analyzing logs` : The practive of collecting logs from different network and sometimes client devices on the network, then performing an automated analysis on them
	- Analysis of logs would involve looking for specific log messages of interests, like with firewall logs 
- Logs analysis systems are configured using user-defined rules to match interesting or aypical log entries
- Normalizing log data is an important step, since logs from different devices and systems may not be formatted in a common way
- `Correlation analysis` : Process of taking log data from different systems and matching events across the systems
- Detailed logging and analysis of logs would allow for detailed reconstruction of the events that led to the compromise
- `Flood guards` : Provide protection against DoS (Denial of Service attacks)

Network Software Hardening
- Includes things like firewalls, proxies, and VPNs
	- i.e. Firewalls : firewalls are critical to securing a network. They can be `deployed as dedicated network infrastructure devices`, which regulate the flow of traffic for a whole network. They can also be `host-based` as software that runs on a client system providing protection for that one host only.
    	- A host-based firewall provides protection for mobile devices such as a laptop that could be used in an untrusted, potentially malicious environment like an airport Wi-Fi hotspot. 
        - Host-based firewalls are also useful for protecting other hosts from being compromised, by corrupt device on the internal network. 
	- i.e. VPNs are also recommended to provide secure access to internal resources for mobile or roaming users
    	- VPNs are commonly used to provide secure remote access, and link two networks securely.
	- Proxies can be really useful to protect client devices and their traffic
    	- They also provide secure remote access without using a VPN
        - A standard web proxy can be configured for client devices. This allows web traffic to be proxied through a proxy server that we control for lots of purposes. This configuration can be used for logging web requests of client devices. The devices can be used for logs, and traffic analysis, and forensic investigation. 
        - The proxy server can be configured to block content that might be malicious, dangerous, or just against company policy. 
        - A reverse proxy can be configured to allow secure remote access to web based services without requiring a VPN.

#### Wireless Security

WEP Encryption and Why You Shouldn't Use it
- `WEP` Wired Equivalent Privacy
- WEP was proven to be seriously bad at providing confidentiality or security for wireless networks
- WEP use `RC4` symmetric stream cipher for encryption

WPA/WPA2
- Wi-Fi Alliance was WPA or Wi-Fi Protected Access : Replacement for WEP
- `WPA` was designed as a short-term replacement that would be compatible with older WEP-enabled hardware with a simple firmware update
- To address the shortcomings of WEP security, a new security protocol was introduced called TKIP or the Temporal Key Integrity Protocol.
- TKIP implemented three new features that made it more secure than WEP. 
	1. more secure key derivation method was used to more securely incorporate the IV into the per packet encryption key. 
    2. sequence counter was implemented to prevent replay attacks by rejecting out of order packets. 
    3. 64-bit MIC or Message Integrity Check was introduced to prevent forging, tampering, or corruption of packets
- WPA2 is the best security for wireless networks currently available; It's based on the AES cipher finally getting away from the insecure RC4 cipher (The key derivation process didn't change from WPA, and the pre-shared key requirements are the same.)
- 4-way handshake : Designed to allow an AP to confirm that the client has the correct pairwise master key, or pre-shared key in a WPA-PSK setup without disclosing the PMK
	- PMK is `long live key` and might not change for a long time. So an encryption key is derived from the PMK that's used for actual encryption and decryption of traffic between a client and AP.
    -  This key is called the Pairwise Transient Key or PTK. 
    -  The PTK is generating using the PMK, AP nonce, Client nonce, AP MAC address, and Client MAC address. 
- WPA supports : 
	1. PIN entry authentication
    2. NFC or USB
    3. Push button authentication

#### Network Monitoring

Sniffing the Network
- `Packet sniffing` (Packet capture) : The process of intercepting network packets in their entirety for analysis
- Promiscuous Mode : A type of computer networking operational mode in which all network data packets can be accessed and viewed by all network adapters operating in this mode
- Port mirroring : Allows the switch to take all packets from a specified port, port range, or the entire VLAN and mirror the packets to a specified switch port
- Monitor mode : Allows us to scan across channels to see all wireless traffic being sent by APs and clients

Wireshark and tcpdump
- `Tcpdump` is a lightweight command-line based utility that you can use to capture and analyze packets.

Intrusion Detection/Prevention Systems
- IDS or IPS systems operate by monitoring network traffic and analyzing it
- They look for matching behavior or characteristics that would indicate malicious traffic.
- The difference between an IDS and an IPS system, is that IDS is only a detection system It won't take action to block or prevent an attack, when one is detected, it will only log an alert. But an IPS system can adjust firewall rules on the fly, to block or drop the malicious traffic when it's detected.
- IDS and IPS system can either be host based or network based. 
- In the case of a `Network Intrusion Detection System` or NIDS, the detection system would be deployed somewhere on a network, where it can **monitor traffic** for a network segment or sub net.

### Week 5

#### System Hardening

Disabling Unnecessary Components
- `Attack vecttor` : Method/Mechanism by which an attacker or malware gains access to anetwork or system
- `Attack surface` : The sum of all the different attack vectors in a given system
- The less complex something is, the less likely there will be undetected flaws
- Another way to keep things simple is to reduce your software deployments
- Defense in depth concept is all about risk mitigation and implementing layers of security.
 
Host-Based Firewall
- Protect individual hosts from being compromised when they're used in untrusted and potentially malicious environments
- A host-based firewall plays a big part in reducing what's accessible to an outside attacker
	- It provides flexibility while only permitting connections to selective services on a given host from specific networks or IP ranges.
    - This ability to restrict connections from certain origins is usually used to implement a highly secure host to network.
    - rom there, access to critical or sensitive systems or infrastructure is permitted. 
    - These are called `Bastion hosts` or networks,
- Good to keep the network that VPN clients connected to separate using both subnetting and VLANs. 
	- This gives you more flexibility to enforce security on these VPN client
- If the users of the system have administrator rights, then they have the ability to change firewall rules and configurations. 

Logging and Auditing
- Need visibility into the security systems in place to see what kind of traffic they're seeing
- SIEMS `Security Information and Event Management System` : Centralized Log server
- Logs analysis is normalization : Process of taking log data in different formats and converting it into a standardized format that's consistent with a defined log structure
- What type of information should you be logging?
	- i.e. Timestamp, event, error code, service or applicatio being logged, user or system account associated with the event, device involved in the event
- Once logs are centralized and standardized, you can write automated alerting based on rules.

Antimalware Protection 
- Lots of unprotected systems would be compromised in a matter of minutes if directly connected to the internet without any safeguards or protections in place.
- `Antivirus software` is **signature based**. This means that it has a database of signatures that identify known malware like the unique file hash of a malicious binary or the file associated with an infection
- `Antivirus software` will monitor and analyze things like new files being created or being modified on the system in order to watch for any behavior that matches a known malware signature. 

Disk Encryption
- `Full-disk Encryption` FDE : Works by automatically converting data on a hard drive into a form that cannot be understood by anyone who doesn't have the key to "undo" the conversation (FDE is key - Systems with their entire hard drives encrypted are resilient against data theft)
- Since disk encryption not only provides confidentiality but also integrity. This means that an attacker with physical access to a system can't replace system files with malicious ones or install malware.
- In order for a system to boot if it has an FDE setup, there are some critical files that must be accessible. They need to be available before the primary disk can be unlocked and the boot process can continue $\to$ Because of this, all FDE setups have an unencrypted partition on the disk, which holds these critical boot files (i.e. kernel, bootloader)
- Secure boot is confifured with what's called a platform key (= public key corresponding to the private kwy used to sign the boot file)
- Password-protecting the key works by requiring the user entry passphrase to unlock the encryption key.
- When you implement a full-disk encryption solution at scale, it's super important to think about how to handle cases where passwords are forgotten. This is another convenience tradeoff when using FDE.
- `Key escrow` : Allows encryption key to be securely stored for later retrieval by an authorized party.
- Home directory or file-based encryption only guarantees confidentiality and integrity of files protected by encryption.

#### Application Hardening

Software Patch Management
- Software updates don't just improve software products by adding new features and improving performance and stability, they also address security vulnerabilities
- The best protection is to have a good system and policy in place for your company -> The system should be checking for, distributing and verifying software updates for software deployment.
- Patching isn't just necessary for software, but also operating systems and firmware that run on infrastructure devices. 
- Operating system vendors usually push security related patches pretty quickly when an issue is discovered.
- But, for embedded devices like networking equipment or printers, this might not be typical.
- Critical infrastructure devices should be approached carefully when you apply updates. There's always the risk that a software update will introduce a new bug that may affect the functionality of a device, or if the update process itself would go wrong and cause an outage.

Application Policies
- Application Policies : (1) Defined boundaries of what applications are permitted or not (2) Help educate folks on how to use software more securely
- Recommended to use lastest version
- It's generally a good idea to disallow risky classes of software by policy. Things like file sharing software and piracy-related software tend to be closely associated with malware infections.
- Understanding what your users need to do their jobs will help shape your approach to software policies and guidelines.
- Helping your users accomplish tasks by recommending or supporting specific software makes for a more secure environment $\to$ It also helps users by giving them clear solutions to accomplish tasks
- Extensions that require full access to web sites visited can be risky since the extension developer has the power to modify pages visited.





 





























