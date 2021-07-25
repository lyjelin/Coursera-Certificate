Jul 25 2021
> 
- Technical support fundamentals
- Computer networking
- Operating systems
- Sys admin & infrastructure services
- IT security

## Technical support fundamentals 

### Week 1

Computer Language
- Binary System - 0s and 1s, bit = binary digits
- Byte = Group of 8 bits
	- Each byte can store 1 character, and we can have 256 possible values, $2^8$
	- `01101000 01100101  01101100  01101100   01101111 = hello`


Character Encoding
- i.e. ASCII table, UTF-8, RGB

Binary
- Logic Gates : Allow tansistors to do more complex tasks
- `128 62 32 16 8 4 2 1`

---

### Week 2

Computer Hardware
- Desktop, Keyboard, Monitors, etc.
- Ports : Connection points that can connect devices to that extend the functionality of computer
- CPU (central processing unit) - brain of computer
- RAM (random access memory) - short-term memory
- Hard drive - long-term memory
- Motherboard - cuircuit board that connects all componenets together

Programs & HW
- EDB (External DataBus)
- MCC : bridge between CPU & RAM
- Addres Bus: connect CPU && MCC
- Cache : used to store frequently accessed data
	- 3 Different cache levelsin CPU : L1, L2, L3
    - L1 smallest + fastest

CPU `Most important part of computer`
- CPU should be compatible with your motherboard 
- CPU sockets (LGA, PGA)
- Prone to overheating - Must connect heat sink
- 32bit/64bit architecture (i.e. 32bit can access $2^{32}$bytes of RAM

RAM
- volatile : clear memory once computer's power off
- i.e. DRAM `Dynamic Random-Access Memory`, SDRAM `Synchronous DRAM`, DDR SDRAM `Double Data Rate SDRAM` 
- **Faster RAM** = programs can be run faster && more programs can run at the same time

Motherboards
- Allows different parts of computer to communicate
- Components 
	- chipset : allows manageing data between CPU, RAM, peripherals
    	- Northbridge : interconnects RAM/video cards
        - SouthBridge : maintains IO controllers (Hard drives, USB devices)
	- peripherals : external devices connected to computer (mouse/keyboard/monitor)
	- Expansion slots : 확장 슬롯 gives ability to increase the functionality of computer
    	- PCI express `Peripheral Component Interconnect Express`
 	- Form factor : 하드웨어 부품의 크기, 모양, 실제 사양 
   - ATX `Advanced Technology eXtended`
  - ITX `Information Technology eXtended` 

Storage
- Data sizes :
	1. 8 bit = 1 byte
    2. 1024 bytes = 1 KB (kilobyte)
    3. 1024 megabytes = 1 MB (megabyte)
    4. 1024 gigabytes = 1 TB (terabyte)
- Storage types
	1. HDD `Hard Disk Drive` (i) more prone to damage (ii) affordable (iii) more bulk
    2. SDD `Solid State Drive` (i) less risky in lossing data (ii) expensive (iii) slimmer form factor
- RPM `revolution per minute` : HD with higher RPM is faster

Mobile Devices
- SoC `System on a Chip` : Packs CUP/RAM and sometimes storage onto a single chip

Peripherals
- USB [reference](https://en.wikipedia.org/wiki/USB)
	- 1 MB = 1 Megabyte | 1 Mps = 1 megabit per second (unit of data transfer rate)
	- 1 byte = 8 bit, hence transfering 1 MB file we need 8 Mbs connection speed
- DVI (outputs video) / HDML & DIsplayPort (video+audio)
- Type C-charger (video+audio+data transfer+power)


BIOS `Basic I/O Services`
- SW that helpd initialize the HW of computer and gets OS up & running
- Motherboard stores BIOS in special type of memory, Read-only Memory (ROM) chip (BIOS settings are stored in CMOS chip)
- UEFI `Unified Extensible Firmware Interface`
- POST `Power On Self Test` : figures out what HW is on computer (**beep**)
- BIOS settings control which devices to boot
- (i) initialize HW (ii) Checks what devices are connected to computer (iii) POST

> Week 2 Graded Assignment
Assemble a Computer $\to$ CPU+thermal paste+heat sink+CPU fan/RAM/Case fan/PSU/HDD/Sata 퍼즐맞추기 너낌쓰 
w2 강의 중 [Putting it all togther](https://www.coursera.org/learn/technical-support-fundamentals/lecture/kHYGB/putting-it-all-together) 다시 참고해서 풀었다. PSU랑 Case fan 위치 헷갈렸지만 패스!

---

### Week 3

#### Operating System

~~Honestly, I don't like operating system. 2학년때 들은 OS 전공수업은 악몽이었...~~

Remote Connection & SSH
- Remote connection : allows us to manage multiple machines (geographically free)
- SSH `Secure Shell` : A protocol implemented by other programs to securely access one computer from another
	- SSH Server/Client
    - SSH Authentication key
    - [Comparison of SSH Clients](https://en.wikipedia.org/wiki/Comparison_of_SSH_clients)
- VPN `Virtual Private Network` : Allows us to connect to a private network (i.e. workbench)


Componenets of an OS
- Whole package that manages our Computer's resources and let users interact with it
	- Window/Linux/MacOS
- Main components :
	1. Kernal : directly talks to HW & Manages our system resources; 
    	- File Storage & Management
        - Process Managements : Allow computer to do multitasking by switching execution of different process on the CPU faster 
        - optimizes **memory usage** and make sure applications have enough memory to run
        - I/O Management
    2. User Space

Files/File Systems
- NTFS : Window's Major file system
- [ReFS](https://en.wikipedia.org/wiki/ReFS) : MS's 
- APFS : MacOS's 
- `Block Storage` improves faster handling of data because the data isn't stored as one long piece and can be accessed quicker

> Kernel : Creates Processes, efficiently schedules them, and manages how processes are terminated

Process Management 
- Process : program that's executing (i.e. internet browser, text editor)
- Program : application that we can learn (i.e. Chrome)
- Time slices

Memory Management
- Virtual memory : The combination of hard drive space & RAM that acts like memoty for processes can use
- Kernel handles the process of taking pages of data and swapping them between RAM and virtual memory.

I/O Management
- Kernel handles all the intercommunications between devices
- i.e. If lack of RAM, can't load up as many processes. If lack of CPU, can't execute processes fast enough

Interacting with OS; User spaces
- Shell (i.e. terminal) `OR` GUI
	- Bash, Bourne Again Shell; Shell is a program that interprets text commands and send them to the OS to execute

Logs
- Files that record system events on our computer

The Boot Process
- Bootloader : small program that loads the OS

	Computer power on > BIOS/UEFI (POST) > Boot Deive selection (bootloader) > OS > Kernel loaded > System Processes > User space

Virtual Machines
- VMs use physical resources like memory, CPU and storage, but they offer the added benefit of running multiple operating systems at once. They're also easier to maintain and provision. 
- USB containing OS should be **bootable**

---

### Week 4

Networking
- Interconnection of Computers
- Web : Information on the internet
- Server/Client
- ISP `Internet Service Provider`
- When sending/receiving data through network, you need to have both IP & MAC address
	- IP address : Computers on network have identifier (i.e. house address)
	- MAC Address (i.e. recipient's name)
- Networking HW
	- ethernet cable
	- WiFi
	- FIbre optic cable (fastest; most expensive)
- Networking Protocol (i.e. `TCP/IP`)
	- IPv4, IPv6
- DNS `Domain Name System` : maps IP adress ito website name
- NAT `Network Address Translation` : Lets organizations use one public IP address and many private IP addresses within the network


> Router : Connects lots of different devices together and helps route network traffic
- Utilizes netwotk protocols to help determine where to send the packet

---

### Week 5

- Coding : translating one language to another
- Scripting : mainly used to perform a single or limited range task
- Programming : coding in `programming language`

> Copyright : Used when creating original work

Types of SW
- Open-source SW
- Applicatio SW : any SW created to fulfill a specific need, like a text editor, web browser, or graphic editor
- System SW : SW used to keep core system running (like OS tools & utilities)
	- Firmware (i.e. `BIOS`): SW that's permanently stored on a computer component
    - MacOS

> [SW Version control](https://en.wikipedia.org/wiki/Software_versioning)

Languages
- Assembly Language 
- Compiled Programming Language : uses human readeable instructions, then sends them through compiler
- Script : is run by interpreter, which interprets the code into CPU instructions just in time to run them

> SW bugs : an error in software that causes unexpected results

Managing Software
1. Installing sw
2. Updating sw
3. Removing sw

---

### Week 6

뭔가 멋진 phrases 

> Fixing problems and creating positive interactions with people are two fundamental skills in IT field

> As an IT support specialist, you're uniquely positioned to combine technology and people how how to make those interactions better, and make a difference in people's day to day lives  

Trobleshooting problems & solid communication
- Troubleshooting : ability to diagnose and resolve a problem
- IT Support is about working in the service of others. Always trys to create a positive experience for the user

Customer Service

- Exhibiting empathy
- Being conscious of tone
- Acknowledging the person
- Developing trust

Anatomy of Interaction $\to$ Be professional, acknowledge the user, show some respect

Documentation
`Ticketing (common way of documenting an issue) OR Bug System (Issues with the system that weren't caused by an external source)`
- Documentation is important as they (i) keeps the user in the loop (ii) helps you audit your steps in case you need to go back and see what you did

