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










