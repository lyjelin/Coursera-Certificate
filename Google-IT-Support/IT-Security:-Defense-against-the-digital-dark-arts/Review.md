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









