# IT Security: Defense against the digital dark arts

## Week 1

### Malicious Software

1. In the CIA Triad, "Confidentiality" means ensuring that data is:
- [ ] available and that people can access it
- [ ] accurate and was not tampered with
- [ ] acessible anonymously
- [x] **not accessible by unwanted parties**

2. In the CIA Traid, "integrity" means ensuring that data is:
- [x] **accurate and was not tampered with**
- [ ] available and that people can access it
- [ ] not accessible by unwanted parties
- [ ] truthful and honest

3. In the CIA Traid, "Availability" means ensuring that data is 
- [ ] available to anyone from anywhere
- [ ] accurate and was not tampered with
- [x] **available and that people can access it**
- [ ] not accessible by unwanted parties

4. What's the relationship between a vulnerability and an exploit?
- [x] **An exploit creates a vulnerability in a system**
- [ ] They're unrelated
- [ ] A vulnerability takes advantage of an exploit to run arbitary code or gain access
- [ ] An exploit takes advantage of a vulnerability to run arbitary code or gain access

5. Which statement is true for both a worm and a virus?
- [ ] They're undetectable by antimalware softeare
- [x] **They're self-replicating and self-propagating**
- [ ] They don't cause any harm to the target system
- [ ] They infect other files with malicious code

6. Check all examples of types of malware:
- [x] **Adware**
- [ ] Key Generators
- [x] **Viruses**
- [x] **Worms**

7. What are the characteristics of a rootkit? Check all that apply.
 - [x] **Provide elevated credentials**
 - [x] **Is difficult to detect**
 - [ ] Is harmless
 - [ ] Is destructive

### Network Attacks

1. What are the dangers of a man-in-the-middle attack? Check all that apply
- [x] **An attacker can modify traffic in transit**
- [x] **An attacker can block or redirect traffic**
- [x] **An attacker can eavesdrop on unencrypted traffic**
- [ ] An attacker can destroy data at rest

2. Why is a DNS cache poisoning attack dangerous? Check all that apply
- [x] **It allows an attacker to redirect targets to malicious webservers.**
- [ ] It allows an attacker to remotely control your computer.
- [ ] Errrr...it's not actually dangerous.
- [x] **It affects any clients querying the poisoned DNS server.**

3. Which of the following is true of a DDoS attack? 
- [ ] Attack traffic is encrypted
- [ ] This type of attack causes a significant loss of data
- [x] **Attack traffic comes from lots of different hosts**
- [ ] An attacker sends attack traffic directly to the target

4. Which of the following result from a denial-of-service attack? Check all that apply.
- [x] **Slow network performance**
- [ ] Malware infection
- [ ] Data destruction
- [x] **Service unreachable**

### Other Attacks

1. How can you protect against client-side injection attacks? Check all that apply.
- [ ] Utilize strong passwords
- [x] **Use input validation**
- [ ] Use a SQL database
- [x] **Use data sanitization**

2. True or false: A brute-force attack is more efficient than a dictionary attack.
- [ ] True
- [x] **False**

3. Which of the following scenarios are social engineering attacks? Check all that apply. 
- [ ] An attacker performs a man-in-the-middle attack.
- [x] **You receive an email with an attachment containing a virus.** 
- [ ] An attacker performs a DNS Cache poisoning attack.
- [x] **Someone uses a fake ID to gain access to a restricted area.**

### Graded Assessments : Understanding Security Threats

1. Which of the following are examples of injection attacks? Check all that apply.
- [ ] SYN flood attack
- [x] **XSS attack**
- [ ] Social engineering attack
- [x] **SQL injection attack**

2. An attacker could redirect your browser to a fake website login page using what kind of attack?
- [ ] DDoS attack
- [ ] Injection attack
- [x] **DNS cache poisoning attack**
- [ ] SYN flood attack

3. An attack that would allow someone to intercept your data as it's being sent or received is called a(n) _________ attack.
- [ ] Injection
- [ ] SYN flood
- [ ] Denial of Service
- [x] **Man-in-the-middle**

4. The best defense against injection attacks is to ______.
- [ ] Use antimalware software
- [x] **Use input validation**
- [ ] Use strong passwords
- [ ] Use a firewall
 
5. The practice of tricking someone into providing information they shouldn't is called ________.
- [ ] Man-in-the-middle attacks
- [ ] Brute force attacks
- [x] **Social engineering**
- [ ] Eavesdropping

6. Which of these is true of vulnerabilities? Check all that apply.
- [x] **An exploit takes advantage of bugs and vulnerabilities**
- [ ] An exploit the possibility of taking advantage of a vulnerability bug in code
- [ ] A vulnerability is the possibility of suffering a loss in the event of an attack
- [x] **A vulnerability is a flaw in the code of an application that can be exploited**

7. Which of these is true of blackhat and whitehat hackers?
- [ ] Blackhats and whitehats shouldn't be trusted
- [ ] Blackhats try to find weaknesses, but whitehats don't
- [x] **Blackhats are malicious. Whitehats exploit weakness to help mitigate threats**
- [ ] Blackhats work with owners to fix problems. Whitehats are just trying to get into a system

8. What is it called when a hacker is able to get into a system through a secret entryway in order to maintain remote access to the computer?
- [ ] Ransomware
- [x] **A backdoor**
- [ ] Adware
- [ ] A Trojan

9. An unhappy Systems Administrator wrote a malware program to bring down the company's services after a certain event occurred. What type of malware does this describe?
- [ ] A rootkit
- [ ] Ransomeware
- [x] **A logic bomb**
- [ ] Spyware

10. What can occur during a ping of death (POD) attack? Check all that apply.
- [x] **Remote code execution**
- [ ] Baiting
- [x] **A Denial-of-Service (DoS)**
- [x] **A buffer overflow**

11. What type of attack can a hacker perform that involves injecting malicious code into a website to hijack a session cookie?
- [ ] Ping flood
- [ ] A password attack
- [ ] SQL injection
- [x] **Cross-site Scripting (XSS)**

12. If a hacker targets a vulnerable website by running commands that delete the website's data in its database, what type of attack did the hacker perform?
- [ ] A dictionary attack
- [x] **SQL injection**
- [ ] A Denial-of-Service (DoS) attack
- [ ] Cross-site Scripting (XSS)

13. You receive a legitimate-looking email from a sender that you recognize asking you to click a funny link. But, once you do, malware installs on your computer. What is most likely the reason you got infected?
- [ ] The sender's email password was cracked
- [ ] The sender's email has been hacked
- [x] **The sender's email was spoofed**
- [ ] The sender's email password was used in a DNS Cache Poisoning attack

## Week 2

### Symmetric Encryption

1. What are the components that make up a cryptosystem? Check all that apply.
- [x] **Key generation algorithms**
- [x] **Decryption algorithms**
- [ ] Transmission algorithms
- [x] **Encryption algorithms**

2. What is steganography
- [ ] The study of stegosauruses
- [ ] The practive of encoding messages
- [x] **The practice of hiding messages**
- [ ] The study of languages

3. What makes an encryption algorithm symmetric?
- [ ] Different keys used for encryption and decryption
- [ ] High speed  
- [x] **The same keys used for encryption and decryption**
- [ ] Very large key sizes

4. What's the difference between a stream cipher and a block cipher?
- [ ] There is no difference
- [x] **Stream ciphers encrypt data as a continuous stream, while block ciphers operate on chunks of data.**
- [ ] Block ciphers are only used for block device encryption.
- [ ] Stream ciphers can't save encrypted data to disk.

5. True or false: The smaller the encryption key is, the more secure the encrypted data is.
- [ ] True 
- [x] False

### Public Key or Asymmetric Encryption

1. Which of the following do asymmetric cryptosystems provide? Check all that apply.
- [x] **Authenticity**
- [x] **Confidentiality**
- [ ] Availability
- [x] **Non-repudiation**

2. What advantages do asymmetric algorithms have over symmetric ones? 
- [ ] They have very fast performance.
- [x] **They allow secure communication over insecure channels**
- [ ] They're easier to implement
- [ ] They're more secure

3. What's a common applicatio for aymmetric algorithm
- [ ] Secure password storage
- [ ] Random number generation
- [ ] Full disk encryption
- [x] **Secure exchange**

### Hashing

1. How is hashing different from encryption?
- [ ] Hashing is meant for large amounts of data, while encryption is meant for small amounts of data.
- [ ] It's faster
- [ ] It's less secure
- [x] **Hashing operations are one-directional**

2.What's a hash collision?
- [ ] When two identical files generate different hash digests
- [ ] When a hash digest is reversed to recover the original
- [ ] When two different hashing algorithms produce the same hash
- [x] **When two different files generate the same hash digest**

3. How is a Message Integrity Check (MIC) different from a Message Authentication Code (MAC)?
- [ ] They're the same thing
- [ ] A MIC is more reliable then a MAC
- [x] **A MIC only hashes the message, while a MAC incorporates a secret key**
- [ ] A MAC requires a password, while a MIC does not

4. How can you defend against brute-force password attacks? Check all that apply.
- [x] **Run passwords through the hashing function multiple times**
- [x] **Incorporate salts into password hashing**
- [x] **Enforce the use of strong passwords**
- [ ] Store passwords in a rainbow table

### Cryptography Applications

1. What information does a digital certificate contain? Check all that apply.
- [ ] Private key data
- [x] **Digital signiture**
- [x] **Identifying information of the certificate owner**
- [x] **Public key data**

2. Which type of encryption does SSL/TLS use?
- [ ] Asymmetric encryption
- [x] **Both**
- [ ] Neither
- [ ] Symmetric encryption

3. What are some of the functions that a Trusted Platform Module can perform? Check all that apply.
- [ ] Malware detection
- [x] **Remote attestation**
- [x] **Data binding and sealing**
- [ ] Secure user authentication

### Graded Assessments :

1. Plaintext is the original message, while _____ is the encrypted message.
- [x] **Ciphertext**
- [ ] Digest
- [ ] Algorithm
- [ ] Cipher

2. The specific function of converting plaintext into ciphertext is called a(n) ______.
- [ ] Permutation
- [ ] Data protection standard
- [ ] Integrity check
- [x] **Encryption algorithm**

3. Studying how often letters and pairs of letters occur in a language is referred to as _______.
- [ ] Codebreaking
- [ ] Espionage
- [ ] Cryptography
- [x] **Frequency analysis**

4. True or false: The same plaintext encrypted using the same algorithm and same encryption key would result in different ciphertext outputs.
- [ ] True
- [x] **False**

5. The practice of hiding messages instead of encoding them is referred to as ______.
- [ ] Encryption
- [ ] Obfuscation
- [ ] Hashing
- [x] **Steganography**

6. ROT13 and a Caesar cipher are examples of _______.
- [ ] Asymmetric encryption
- [ ] Steganography
- [ ] Digiral signitures
- [x] **Substitution ciphers**

7. DES, RC4, and AES are examples of ______ encryption algorithms.
- [ ] Asymmetric
- [ ] Strong
- [ ] Weak
- [x] **Symmetric**

8. What are the two components of an asymmetric encryption system, necessary for encryption and decryption operations? Check all that apply.
- [x] **Public key**
- [ ] Digest
- [x] **Private key**
- [ ] Random number generator

9. To create a public key signature, you would use the ______ key.
- [x] **Private**
- [ ] Public
- [ ] Decryption
- [ ] Symmetric

10. Using an asymmetric cryptosystem provides which of the following benefits? Check all that apply.
- [ ] Hashing
- [x] **Confidentiality**
- [x] **Authenticity**
- [x] **Non-repudiation**

11. If two different files result in the same hash, this is referred to as a ________.
- [ ] Coincidence
- [x] **Hash collision**
- [ ] Mistake
- [ ] Key collision

12. When authenticating a user's password, the password supplied by the user is authenticated by comparing the \____ of the password with the one stored on the system.
- [x] **Hash**
- [ ] Plaintext
- [ ] Ciphertext
- [ ] Length

13. If a rainbow table is used instead of brute-forcing hashes, what is the resource trade-off?
- [x] **Rainbow tables use less computational resources and more storage space**
- [ ] Rainbow tables use less storage space and more RAM resources
- [ ] Rainbow tables use less RAM resources and more computational resources
- [ ] Rainbow tables use less storage space and more computational resources

14. In a PKI system, what entity is responsible for issuing, storing, and signing certificates?
- [ ] Government
- [ ] Registration Authority
- [x] **Certificate Authority**
- [ ] Intermediary Authority

## Week 3

### Authentication

1. How is authentication different from authorization?
- [ ] Authentication is identifying a resource; authorization is verifying access to an identity
- [ ] They're the same thing
- [ ] Authenticatio is verifying access to a resource; authorization is verifying an identity.
- [x] **Authentication is verifying an identity; authorization is verifying access to a resource.**

2. What are some characteristics of a strong passwrod? Check all that apply.
- [ ] Contains dictionay words
- [ ] Is used across accounts and systems
- [x] **Includes numbers and special characters**
- [x] **Is at least eight characters long**

3. In a multi-factor authentication scheme, a password can be thought of as: 
- [ ] somthing you are
- [ ] something you have.
- [ ] something you use.
- [x] **something you know.**

4. What are some drawbacks to using biometrics for authentication? Check all that apply. 
- [x] **There are potential privacy concerns.**
- [x] **Biometric authentication is difficult or impossible to change if compromised.**
- [ ] Biometric authentication is much slower than alternatives.
- [ ] Biometrics are easy to share.

5. In what way are U2F tokens more secure than OTP generators? 
- [ ] They're cheaper
- [x] **They're resistant to phishing attacks.**
- [ ] They can't be cloned.
- [ ] They're password-protected.

6. What elements of a certificate are inspected when a certificate is verified? Check all that apply. 
- [x] **Trust of the signatory CA**
- [ ] Certificate key size
- [x] **"Not valid before" date**
- [x] **"Not valid after" date**

7. What is a CRL? 
- [ ] Certified Recursive Listener
- [x] **Certificate Revocation List**
- [ ] Caramel Raspberry Lemon
- [ ] Certificate Recording Language

8. What are the names of similar entities that a Directory server organizes entities into?
- [ ] Clusters
- [x] **Organizational Units**
- [ ] Trees
- [ ] Groups

9. True or false: The Network Access Server handles the actual authentication in a RADIUS scheme.
- [ ] True
- [x] **False**

10. True or false: Clients authenticate directly against the RADIUS server.
- [ ] True
- [x] **False**

11. What does a Kerberos authentication server issue to a client that successfully authenticates? 
- [x] **A ticket granting ticket**
- [ ] An encryption key
- [ ] A master password
- [ ] A digital certificate

12. What advantages does single sign-on offer? Check all that appl
- [ ] It provides encrypted authentication
- [x] **It reduces the total number of credentials**
- [x] **It reduces time spent authenticating**
- [ ] It enforces multifactor authentication

13. What does OpenID provide? 
- [ ] Digital signiture
- [x] **Authentication delegation**
- [ ] Certificate signing
- [ ] Cryptographic hashing

### Authorization and Accounting

1. What role does authorization play? 
- [x] **It determines whether or not an entity has access to a resource.**
- [ ] It verifies an entity's identity. 
- [ ] It verifies passwords. 
- [ ] It provides strong encryption.

2. What does OAuth provide? 
- [ ] Confidentiality
- [ ] Integrity
- [x] **Access delegation**
- [ ] Secure communications

3. How is auditing related to accounting? 
- [ ] They're not related
- [ ] They're the same thing
- [ ] Accounting is reviewing records, while auditing is recording access and usage
- [x] **Accounting is record access and usage, while auditing is reviewing these records**

### Graded Assessments : AAA Security (Not Roadside Assistance)

1. Authn is short for ________.
- [ ] Authotization
- [ ] Authoritarian
- [ ] Authored
- [x] **Authentication**

2. Authorization is concerned with determining ______ to resources.
- [x] **Access**
- [ ] Eligibility
- [ ] Validity
- [ ] Identity

3. In addition to the client being authenticated by the server, certificate authentication also provides ______.
- [x] **Server authentication**
- [ ] Authorization
- [ ] Malware protection
- [ ] Integrity

4. The authentication server is to authentication as the ticket granting service is to _______.
- [ ] Integrity
- [x] **Authorization**
- [ ] Verification
- [ ] Identification

5. Which of these passwords is the strongest for authenticating to a system?
- [ ] P@55w0rd!
- [x] **P@w04d!$$L0N6**
- [ ] P@ssword!
- [ ] Password!

6. In a Certificate Authority (CA) infrastructure, why is a client certificate used?
- [x] **To authenticate the client**
- [ ] To authenticate the subordinate CA
- [ ] To authenticate the server
- [ ] To authenticate the CA

7. A network admin wants to use a Remote Authentication Dial-In User Service (RADIUS) protocol to allow 5 user accounts to connect company laptops to an access point in the office. These are generic users and will not be updated often. Which of these internal sources would be appropriate to store these accounts in?
- [ ] SQL database
- [ ] LDAP
- [ ] Active Directory
- [x] **Flat file**

8. Kerberos enforces strict _____ requirements, otherwise authentication will fail.
- [x] **Time**
- [ ] AES
- [ ] NTP
- [ ] Strong password

9. Which of these are examples of a Single Sign-On (SSO) service? Check all that apply.
- [x] **OpenID**
- [ ] Tokens
- [ ] Relying Parties
- [ ] Kerberos
> I didn't select all the correct answers


10. A company is utilizing Google Business applications for the marketing department. These applications should be able to temporarily access a user's email account to send links for review. Why should the company use Open Authorization (OAuth) in this situation
- [ ] Utilize a Key Distribution Center server
- [x] **Compatibility with third party apps**
- [ ] Administrater multiple network devices
- [ ] Gain access through a wireless access point

11. Access control entries can be created for what types of file system objects? Check all that apply.
- [x] **Files**
- [x] **Folders**
- [ ] APIs
- [x] **Programs**

## Week 4

### Secure Network Software

1. Why is normalizing log data important in a centralized logging setup? 
- [ ] The data must be decrypted before sending it to the log server
- [ ] It's difficult to analyze abnormal logs
- [ ] Log normalizing detects potential attacks
- [x] **Uniformly formatted logs are easier to store and analyze**

2. What type of attacks does a flood guard protect against? Check all that apply. 
- [ ] Malware infections
- [x] **DDoS attacks**
- [x] **SYN floods**
- [ ] Man-in-the-middle attacks

3. What does DHCP Snooping protect against? 
- [ ] Data theft
- [x] **Rogue DHCP server attacks**
- [ ] DDoS attacks
- [ ] Brute-force attacks

4. What does Dynamic ARP Inspection protect against? 
- [ ] Malware infections
- [ ] Rogue DHCP server attacks
- [ ] DDoS attacks
- [x] **ARP poisoning attacks**

5. What does IP Source Guard protect against?
- [ ] Brute-force attacks
- [ ] Rogue DHCP server attacks
- [x] **IP spoofing attacks**
- [ ] DDoS attacks

6. What does EAP-TLS use for mutual authentication of both the server and the client? 
- [ ] One-time passwords
- [ ] Biometrics
- [x] **Digital certificates**
- [ ] Usernames and passwords

7. Why is it recommended to use both network-based and host-based firewalls? Check all that apply. 
- [x] **For protection against compromised hosts on the same network** 
- [x] **For protection for mobile devices, like laptops**
- [ ] For protection against DDoS attacks
- [ ] For protection against man-in-the-middle attacks

### Wireless Security

1. What are some of the weaknesses of the WEP scheme? Check all that apply. 
- [ ] Its use of ASCII characters for passphrases 
- [x] **Its poor key generation methods**
- [x] **Its small IV pool size**
- [x] **Its use of the RC4 stream cipher**

2. What symmetric encryption algorithm does WPA2 use? 
- [ ] DES
- [ ] DSA
- [ ] RSA
- [x] **AES**

3. How can you reduce the likelihood of WPS brute-force attacks? Check all that apply. 
- [x] **Disable WPS**
- [x] **Implement lockout periods for incorrect attemps**
- [ ] Update firewall rules
- [ ] Use a very long and complex passphrase

4. Select the most secure WiFi security configuration from below: 
- [ ] None
- [ ] WPA enterprise
- [ ] WEP 128
- [ ] WPA personal
- [ ] WPA2 personal
- [x] **WPA2 enterptise**

### Network

1. What does tcpdump do? Select all that apply. 
- [ ] Encrypts your packets
- [x] **Analyzes packets and provides a textual analysi**
- [x] **Captures packets**
- [ ] Generates packets

2. What does wireshark do differently from tcpdump? Check all that apply. 
- [ ] It can capture packets and analyze them. 
- [x] **It has a graphical interface.**
- [ ] It can write packet captures to a file. 
- [x] **It understands more application-level protocols.**

3. What factors should you consider when designing an IDS installation? Check all that apply. 
- [x] **Traffic bandwidth**
- [ ] OS types in use
- [ ] Internet connection speed
- [x] **Storage capacity**

4. What is the difference between an Intrusion Detection System and an Intrusion Prevention System? 
- [ ] They are the same thing
- [ ] An IDS can detect malware activity on a network, but an IPS can't
- [ ] An IDS can actively block attack traffic, while an IPS can only alert on detected attack traffic
- [x] **An IDS can alert on detected attack traffic, but an IPS can actively block attack traffic**

5. What factors would limit your ability to capture packets? Check all that apply.
- [x] **Network interface not being in promiscuous or monitor mode**
- [ ] Anti-malware software
- [ ] Encryption
- [x] **Access to the traffic in question**

### Week Four Practice Quiz

1. What traffic would an implicit deny firewall rule block?
- [ ] Nothing unless blocked
- [ ] Inbound traffic
- [ ] Outbound traffic
- [x] **Everything not allowed**

2. The process of converting log entry fields into a standard format is called _______.
- [x] **Log normalization**
- [ ] Log encryption
- [ ] Log analysis
- [ ] Log auditing
 
3.A ______ can protect your network from DoS attacks.
- [x] **Flood Guard**
- [ ] DHCP 
- [ ] Dynamic ARP inspection
- [ ] IP Source Guard

4. Using different VLANs for different network devices is an example of _______.
- [x] **Network Seperation**
- [ ] Implicit Denial
- [ ] Remote Access
- [ ] Network Encryption

5. How do you protect against rogue DHCP server attacks?
- [ ] Dynamic ARP Inspection
- [ ] IP Source Guard
- [x] **DHCP Snooping**
- [ ] Flood Guard

6. What does Dynamic ARP Inspection protect against?
- [ ] Rogue DHAP Server attacks
- [ ] DoS attacks
- [ ] IP Spoofing attacks
- [x] **ARP Man-in-the-middle attacks**

7. What kind of attack does IP Source Guard protect against?
- [ ] ARP Man-in-the-middle attacks
- [x] **IP Spoofing attacks**
- [ ] Rogue DHAP Server attacks
- [ ] DoS attacks

8.A reverse proxy is different from a proxy because a reverse proxy provides ______.
- [ ] Privacy
- [ ] DoS protection
- [ ] Authentication
- [x] **Remote Access**

9. What underlying symmetric encryption cipher does WEP use?
- [x] **RC4**
- [ ] AES
- [ ] DES
- [ ] RSA

10. What key lengths does WEP encryption support? Check all that apply. 
- [ ] 40-bit
- [x] **64-bit**
- [x] **128-bit**
- [ ] 256-bit

11. What's the recommended way to protect a WPA2 network? Check all that apply.
- [x] **Use a long, complex passphrase**
- [x] **Use a unique SSID**
- [ ] Hide the SSID
- [ ] Use WEP64

12. If you're connected to a switch and your NIC is in promiscuous mode, what traffic would you be able to capture? Check all that apply.
- [ ] All traffic on the switch
- [x] **Broadcast traffic**
- [ ] No traffic
- [x] **Traffic to and from you machind**

13. What could you use to sniff traffic on a switch?
- [ ] Promiscuous Mode
- [ ] Network hub
- [ ] DHCP Snooping
- [x] **Port Mirroring**

14. What does tcpdump do?
- [ ] Handles packet injection
- [ ] Generates DDoS attack traffic
- [ ] Brute forces password databases
- [x] **Perform packet capture and analysis**

15. Compared to tcpdump, wireshark has a much wider range of supported _______.
- [ ] Packet sizes
- [x] **Protocols**
- [ ] Packet types
- [ ] Languages

16. A Network Intrusion Detection System watches for potentially malicious traffic and _______ when it detects an attack
- [ ] Blicks traffic
- [ ] Shuts down
- [ ] Disables network access
- [x] **Triggers alerts**

17. What does a Network Intrusion Prevention System do when it detects an attack?
- [x] **It blocks the traffic**
- [ ] It does nothing
- [ ] It attacks back
- [ ] It triggers an alert

## Week 5

### System Hardening

1. What is an attack vector?
- [x] **A mechanism by which an attacker can interact with your network or systems**
- [ ] The severity of the attack
- [ ] The classification of attack type
- [ ] The direction an attack is going in

2. Disabling unnecessary components serves which purposes? Check all that apply.
- [ ] Increasing performance
- [ ] Making a system harder to use
- [x] **Closing attack vectors**
- [x] **Reducing the attack surface**

3. What's an attack surface? 
- [ ] The payload of the attack
- [ ] The target or victim of an attack
- [ ] The total scope of an attack
- [x] **The combined sum of all attack vectors in a system or network**

4. A good defense in depth strategy would involve deploying which firewalls? 
- [ ] Network-based firewalls only 
- [ ] No firewalls 
- [x] **Both host-based and network-based firewalls**
- [ ] Host-based firewalls only 

5. Using a bastion host allows for which of the following? Select all that apply.
- [x] **Applying more restrictive firewall rules** 
- [ ] Running a wide variety of software securely
- [x] **Enforcing stricter security measures** 
- [x] **Having more detailed monitoring and logging** 

6. What benefits does centralized logging provide? Check all that apply. 
- [x] **It allows for easier logs analysis.** 
- [ ] It prevents database theft. 
- [x] **It helps secure logs from tampering or destruction.**
- [ ] It blocks malware infections. 

7. What are some of the shortcomings of antivirus software today? Check all that apply. 
- [x] **It can't protect against unknown threats.** 
- [ ] It only detects malware, but doesn't protect against it.
- [ ] It's very expensive. 
- [ ] It only protects against viruses. 

8. How is binary whitelisting a better option than antivirus software? 
- [ ] It's not better. It's actually terrible.
- [ ] It has less performance impact. 
- [ ] It's cheaper. 
- [x] **It can block unknown or emerging threats.** 

9. What does full-disk encryption protect against? Check all that apply. 
- [x] **Data theft**
- [ ] IP spoofing attacks
- [ ] Malware infections
- [x] **Tampering with system files**

10. What's the purpose of escrowing a disk encryption key? 
- [ ] Preventing data theft
- [ ] Protecting against unauthorized access
- [x] **Performing data recovery**
- [ ] Providing data integrity

### Application Hardening

1. Why is it important to keep software up-to-date? 
- [x] **To address any security vulnerabilities discovered**
- [ ] To ensure compatibility with other systems 
- [ ] It's not important. It's just annoying. 
- [ ] To ensure access to the latest features 

2. What are some types of software that you'd want to have an explicit application policy for? Check all that apply.
- [ ] Software development kits
- [x] **Filesharing software**
- [ ] Word processors 
- [x] **Video games**















