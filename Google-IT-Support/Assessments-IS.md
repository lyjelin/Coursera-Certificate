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








