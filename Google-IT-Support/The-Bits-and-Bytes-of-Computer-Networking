Jul 27 2021

> 
- Technical support fundamentals
- **The Bits and Bytes of Computer Networking**
- Operating Systems and You: Becoming a Power User
- System Administration and IT Infrastructure Services
- IT Security: Defense against the digital dark arts

Modern Network Configuration
1. IP address
2. Subnet mask
3. Gateway for a host
4. DNS server

## The Bits and Bytes of Computer Networking

### Week 1

TCP/IP 5-layer Networking Model

> OSI `Open Systems Interconnection model` [reference](https://en.wikipedia.org/wiki/OSI_model)

`Lowest` Physical | Data Link | Network | Transport | Application `Highest`

1. Physical - interconnect computers
2. Data Link (Network access layer) - responsible for getting data across a single link
3. Network - allow different networks to communicate with each other through devices known as routers; responsible for getting data delivered across a collection of networks
	- Internetwork : collection of networks connected through routers (i.e. internet)
    - Server / Client
4. Transport - sorts out which client and server programs are supposed to get that data (`TCP/IP`, `UDP`)
5. Application

Basic Networking device

1. Cables : copper & fibre
	- Copper wire 
    	- Sending device communicates **binary data** across the copper wires by **changing the voltage** between two ranges. The receiving end is able to interpret these voltage changes as binary ones and zeros
        - cat5, cat5e, cat6
    	- crosstalk : electric pulse on one wire is accidentally detected on another wire
        - cheaper
	- Fiber
    	- Use pulses of light to represent the ones and zeros of the underlying data
        - faster transmission rate over copper wire
        - travel longer distance
        - more expensive
2. Hubs & Switches (LAN `Local Area Network`)
	- Hub : Physical layer (layer 1) device that allows for connections from many computers at once
    - Switch : Data link layer (layer 2) device
    	- inspect Ethernet data to determine where to send things
3. Routers - Network layer (layer 3) device forwarding data between independent networks
	- inspect IP data to determine where to send things
    - Border Gateway Protocol : Routers share data with each other via BGP, which lets them learn about the most optimal paths to forward traffic
4. Servers & Clients
	- Server : Provides data according to the request(s) received
    - Client : Request data to Server and receive data

#### Physical Layer
- Consist of devices and means of transmitting `bits` across computer networks
- Bit : 0 or 1 (send through wires via modulation)
- Modulation ($\approx$ line coding) : way of varying the voltage of this charge moving across the cable
- [Twisted Pair Cabling](https://en.wikipedia.org/wiki/Ethernet_over_twisted_pair) : twisted nature helps protect against electromagnetic interference and crosstalk from neighboring pairs
- Deplex communication : bi-directional flow of information 
	- Simplex = unidirectional
    - Half deplex : bidirectional but only one device can 'talk' at a time


#### Data Link Layer
- Ethernet - solved collision domains by using CSMA/CD `carrier sense multiple access with collision detection` 
	- CSMA/CD is used to determine when the communications channels are clear, and when device is free to transmit data
    1. If there's no data currently being transmitted on the network segment, a node will feel free to send data
    2. If it turns out that two or more computers end up trying to send data at the same time, the computers detect this collision and stop sending data
    3. Each device involved with the collision then waits a random interval of time before trying to send data again
    4. This random interval helps to prevent all the computers involved in the collision from colliding again the next time they try to transmit anything
- MAC address `Media Access Control address` : globally unique identifier attached to individual network interface (48bit number with hexadecimal numbers)
	- 6 octets
	- First 3 octets of MAC address = OUI `Organizationally Unique Identifier`
- Unicast : just 1 receiving address; if the least significant bit in the first octent of destination address = **0**, means that ethernet frame is intended for only the destination address
- Multicast : if the **least significant bit** in the first octent of destination address = **1**; Multicast frames will be accepted or discarded by each device depending on criteria aside from their own hardware MAC address
- Broadcast 
	- ethernet broadcast address (used so devices can learn more about each other) = FF:FF:FF:FF 
- Dissecting an Ethernet frame 
	- **Data packet** : All-encompassing term that represents any single set of binary data being sent across a network link
    - Ethernet frame : highly structured collection of information presented in a specific order
    - Checksum && CRC

> Ethernet only reports data integrity not data recovery

---
### Week 2

#### Network Layer

IP addresses in dotted deciaml notation

	12.34.56.78
    00001100.00100010.00111000.01001110

- IP addresses belongs to network, not to the devices attached to those network
- DHCP `Dynamic Host Configuration Protocol` : technology that automatically assigns IP address when new device is connected
	- IP address added with DHCP = Dynamic IP address (reserved for clients)
    - Others = Static IP address (reserved for servers & network devices)

IP Datagram 

![](https://images.velog.io/images/elin16/post/4e51231d-1b05-432b-8698-f0450c8a8706/ipDatagram.png)

> IP addresses = network ID + host ID
i.e. 9.100.100.100 $\to$ 9 = network ID, 100.100.100 = host ID

Address class System : Address classes give the way to break the total global IP space into discrete networks
Given 123.456.890.00 :

1. Class A (max host : 16M)
	first octet (123) is used for network ID
2. Class B (max host : 64K)
	first two octets (123.456) are used for network ID
3. Class C (max host : 254)
	first three octets (123.456.780) are used for network ID

Address Resolution Protocol : Protocol used to discover the HW address of a node with a certain IP address

Subnetting : Process of taking large network and splitting it up into many individual and smaller subnetworks/subnets
1. Once your packet gets to the gateway router for the 9.0.0.o Class A network, that router is now responsible for getting that data to the proper system by looking at the host ID. 
2. This is where subnetting comes in. 
3. Subnets can your large network up into many smaller ones. Individual subnets will all have their own gateway routers serving as the ingress and egress point for each subnet.


Subnet masks : 32bit number normally written out as four octets in decimal
Given an IP address (i.e. 10.0.1.10), with subnet, it is consisting of network/subnet/host IDs

![](https://images.velog.io/images/elin16/post/7ec991d1-d6f1-4687-981a-bf94f8359b9f/subnetMasking.png)

CIDAR `Classless Inter-Domain Routing`
- Demarcation point : To describe where one network or system ends and another one begins

#### Routing 


- Router : network device that forwards traffic depending on the destination address of that traffic
- At least two interfaces
- Basic routing : Finding the quickest path to destination networks
	1. Receive data packet
    2. Examines destination IP
    3. Looks up IP destination network in routing table
    4. Forwarding traffic to destination
- Routing Table
- Routing Protocols
	1. Interior Gateway Protocol : used by routers to share information within a single autonomous system
    	- Link state routing protocol
        - Distance-vector protocols (only have neighbour's info)
    2. Exterior Gateway Protocol : used to communicate data between routers representing the edges of an autonomous system
- IANA ` Internet Assigned Numbers Authority`
	1. Managing IP address allocation
    2. Responsible for ASN `Autonomous System Number` allocation
- [Non-routable Address Space](https://www.geeksforgeeks.org/non-routable-address-space/)
	- RFC 1918 (published on 1996) : outlined a number of networks that would be defined as non-routable address space
    - Primary 3 ranges of non-routable space (reserved for private networks, interior gateway protocols will route these spaces within network):
    	- 10.0.0./8 ( Range: 10.0.0.0 – 10.255.255.255 )
        - 172.16.0.0/12 ( Range: 172.16.0.0 – 172.31.255.255 )
        - 192.168.0.0/16 ( Range: 192.168.0.0 – 192.168.255.255 )

> Autonomous System : Collection of networks that fall under the control of a single network operator

---

### Week 3

#### Transport Layer

Multiplexing & Demultiplexing

	Multiplexing : nodes on the network have the ability to direct traffic toward many different receiving services
    
	Demultiplexing : same concept, just at the receiving end, it's taking traffic that's all aimed at the same node and delivering it to the proper receiving service

- Transport layer handles multiplexing & Demultiplexing through ports
- Port : 16-bit number that's used to direct traffic to specific services running on a networked computer

![](../image/multiplexing-demultiplexing.png)

> Ethernet ( IP Datagram ( TCP Segment ) ) )
Ethernet's payload section = entire content of IP datagram
IP Datagram's payload section = made up with TCP segment

TCP (connection-oriented protocol)
1. TCP Segments - made up with header + data section (payload area)
	- source/destination : each 16 bit
	- seq # : 32 bit - helps keep track of the many segments
	- ACK # : 32 bit
	- data offset : 4 bit (contains TCP header length info)
	- TCP window : 16 bit
	- checksum : 16 bit 
2. TCP control flags (6 bit)
	- `URG` : `value = 1` means the segment is considered urgent & urgent pointer field has more data about this
    - `ACK` : `value = 1` means ack field should be checked
    - `PSH` : `value = 1` means transmitting device wants the receiving device to push _currently buffered data_ to the application on the receiving end asap
    - `RST` : `value = 1` means one of the sides in TCP connection hasn't been able to properly recover from series of missing/malformed segments
    - `SYN` : `value = 1` means TCP connection is established and makes sure the receiving end knows to examine the seq # field
    - `FIN` : `value = 1` means TCP connection closed
3. TCP Connections 
	- 3-way handshake
		![]((../image/3wayHandshake.png)
    - 4-way handshake
    	![]((../image/4wayHandshake.png)
4. TCP sockets : instantiation of an end-point in a potential TCP connection
	`Instantiation is the actual implementation of something defined elsewhere`
    - Sockets require actual programs to be instantiated
    - `LISTEN` : socket is ready and listening for incoming connections
    - `SYN_SENT` : synchronization request has been sent, but connection not established yet
    - `SYN-RECEIVED` : socket previously in `LISTEN` state has received `SYN_SENT` and sent `SYN/ACK` back
    - `Established` : TCP connection workong properly
    - `FIN_WAIT` : `FIN` sent but `ACK` not received from the other side
    - `CLOSE_WAIT` : connection closed but application that opened the socket hasn't released its hold on socket yet
    - `CLOSED` : connection fully terminated

UDP (connectionless protocol)
- Set destination port and just send it
- i.e. video streaming

> **TCP VS UDP**
- TCP more reliable 
- UCP faster

Firewall : device that blocks traffic that meets certain criteria
- Firewalls keep a network secure as they are the primary way that can stop traffic user doesn't want from entering a network.

#### Application Layer

TCP segment's payload section

---

### Week 4

#### 1. Domain Name System

- Not efficient to remember MAC or IP address
- Give convenience to end-user (users no need to do any administrative change)
- DNS will be helpful to effectively troubleshoot networking issue

> 
- DNS is a system that converts domain names into IP addresses `Name resolution`
- Used UDP as transport protocal 

DNS servers
1. `Caching name servers` - store known domain name lookups for certain amount of time
2. `Recursive name servers` - perform full DNS resolution requests
- Anycast : technique that's used to route traffic to different detinations depending on factors like location/congestion/link health
 - How recursive name servers operate : 
    	
        User's computer > 
        Caching/recursive name server > 
        (13) root server > 
        Caching/recursive name server > 
        TLD name servers > 
        Caching/recursive name server > T
        housands of name server > 
        Caching/recursive name server > 
        User's computer

DNS Resource Record Types
1. `A record` is used to point a certain domain name at a certain IPv4 IP address - Use round robin method to balance traffic
2. `AAAA (Quad A)` - similar to `A record` but returns IPv6
3. `CNAME` used to redirect traffic from one domain name to another
4. `MX` used for mail exchange
5. `SRV` used for (general) service exchange 
6. `TXT` for texts

Anatomy of Domain name
1. Top level domain name
	- Last part: i.e. `.com` `.org` `.edu`
2. Domain : used to demarcate where control moves from a TLC name server to an authoritative name server
	- i.e. `google` from www.google.com
3. Subdomain = `www`

> Fully Qualified Domain Name - when 1) + 2) + 3) 
$\to$ DNS can support up to 127 levels of domain in total for a single fully FQDN, each individual section can only be 63 characters long, and a complete FQDN is limited to a total of 255 characters

DHCP `Dynamic Host Configuration Protocol` - An Application layer protocol that automates the configuration process of hosts on a network
- Dynamic allocation : range of IP addresses is set aside for client devices and one of these IPs is issued to these devices when they request on
- Automatic allocation : range of IP addresses is set aside for assignment purposes 
- Fixed allocation : requires a manually specified list of MAC address and their corresponding IPs

1. DHCP discovery - The process by which a client configured to use DHCP attempts to get network configuration information 
	![]((../image/DHCP-discover.png)
2. DHCP offer 
	![]((../image/DHCP-offer.png)
3. DHCP request
	![]((../image/DHCP-request.png)
4. DHCP ack
	![]((../image/DHCP-ACK.png)

#### 2. NAT

>NAT `Network Address Translation` is a technology that allows a gateway, usually a router or firewall, to rewrite the source IP of an outgoing IP datagram while retaining the original IP in order to rewrite it into the response

![]((../image/NAT.png)

RIR `Regional Internet Registeris`
1. AFRINIC - continent of Africa
2. ARIN - US, Canada, parts of Caribbean
3. APNIC - Asia, Australia, New Zealand, Pacific island nations
4. LANIC - Central/South America, other parts of Caribbean not covered by ARIN
5. RIPE - Europe, Russia, Middle East, + portion of central Asia

#### 3. VPN & Proxies

VPN : allows for the extension of a private/local network to hosts that might not be on that local network

![]((../image/router.png)

Proxy service : service that acts on behalf of a client in order to access another service
- Anonymity/Security/Content filtering/Increased performance
- i.e. Web proxy 
	![]((../image/webProxy.png)
- i.e. Reverse proxy - service that might appear to be a single server to external clients, but actually represents many servers living behind it
---

### Week 5

POTS and Dial-up
- POTS = `Public Switched Telephone Network`
- Dial-up connection - uses POTS for data transfer, and ets its name because the connection is established by actually dialing a phone number
- Baude rate - measurement of how many bits can be passed across a phone line in a second

#### Broadband connections 광대역
- Broadband means any connectivity technology that isn't dial-up internet
- `T-carrier technology` : transmit multiple phone calls over a single link
	- require dedicated line (mainly used for business purposes)
    - T1 (first T-carrier specification) 
    	- carried up to 24 simultaneoud phone calls across a single piece of twisted pair copper
        - Transmission rate : 1.544 megabits per second
    - T3 = 28 * T1 (all mutiplexed, achieving total throughput speed of 44.736 megabits per second)


Digital Subscriber Lines
- Uses DSLAM `Digital Subscriber Line Access Multiplexers` : establish data connections across phone lines; more long-running
- ADSL `Asymmetric Digital Subscriber Line` : faster download speed, slower upload speed
	![](https://images.velog.io/images/elin16/post/a5ae355e-5bf3-49d4-aa4e-0233b31bf0b8/asdl.png)
- SDSL `Symmetric Digital Subscriber Line` : same upload & download speed
- HDSL `High Bit-rate Digital Subscriber Line`


Cable Broadband has **shared bandwidth technology** and usually managed by cable modem. 

> Cable modem is the device that sits at the edge of a consumer's network and connects it to the cable modem termination system `CMTS`, where `CMTS` connects lots of different cable connections to an ISPs core network

Fibre Connections
- Allows for transmittion to trabel mush further **without** degradation of signal
- Use light for data transmission
- `FTTX` Fiber to the X
    - `FTTP` Fiber to the Premises
    	- `FTTB` Fiber to the Building
    	- `FTTH` Fiber to the Home
    - `FTTN` Fiber to the Neighbour
- ONT `Optical Network Terminator` is known as the demarcation point for Fiber Technology
	- Converts data from protocols the fiber network can understand, to those that more traditional, twisted-pair copper networks can understand

#### WAN (Wide Area Network)

- Acts like a single network, but spans across multiple physical locations
- Usually require user to contract a link across the Internet with ISP; ISP handles sending user data from one site to the other
- Typical WAN setup has a few sections : 
	1. Imagine one network of computers on one side of the country and another network of computers on the other
    2. Each of those networks ends at a demarcation point, which is where the ISP's network takes over
    3. The area between each demarcation point and the ISP's actual core network is called a `local loop` (something like a T-carrier line or a high speed optical connection to the provider's local regional office)
    4. From there, it would connect out to the ISP's core network and the Internet at large
    5. WANs work by using a number of different protocols at the **data link layer** to transport your data from one site to another. 
- Point-to-Point VPNs : establish VPN tunnel setup, which is handled by network devices, between two sites

#### Wireless Networking Technologies

- IEEE 802.11 standards : specifications for how wireless networking devices should communicate; make up the set of WiFi
	- 802.11b, 802.11a, 802.11g, 802.11n, 802.11ac
- 802.11 protocols as defining how we operate at both the physical and the data link layers
- Frequency band : certain section of the radio spectrum that's been agreed upon to be used for certain communications
	- FM broadcast band
    - WiFi network (2.4Ghz, 5Ghz)
- `802.11 frame`'s field
	- frame control field `16 bit` & contains number of subfields that are used to describe how the frame itself should be processed
    - Duration field : specified how long the total frame is, so receiver knows how long it should expect to have to listen to this transmission
    - MAC address header : consists of 
    	- Address 1 - source address field
        - Address 2 - intended destination
        - Address 3 - receiving address
        - Sequence control `16 bit` & contains seq# used to keep track of ordering of frames
        - Address 4 - transmitter address
        - Data payload - has all the data of the protocols further up the stack
        `+ In lots of situations, 
        destination = receiver address`
    - Frame check sequence field : contains checksum used for `CRC`
- Wireless access point : device that bridges the wireless and wired portion of a network

Wireless Network Configurations

1. Ad-hoc networks 
- no supporting network infrastructure
- every device involved with the network communicates with every other device within range and all nodes help pass along messages
- i.e. airdrop, bluetooth

2. Wireless LANS
- consists of 1 or more access points, which acts as bridges between the wireless and wired networks
    ![]((../image/WLAN.png)

3. Mesh Network
- Made up of only wireless access points
- This kind of network allow to deploy more access points to the mesh without having to run a cable to each of them

Wireless Channels

- Channels are individual, smaller sections of the overall fequency band used by wireless network
- Morden wireless networking equipment is built to auto sense what channels are most congested
- Switches remember which computers live on which physical interfaces

> understanding how these channels overlap for all of the 802.11 specifications is a way you can help troubleshoot bad wireless connectivity problems or slowdowns in the network.

Wireless Security

- WEP `Wired Equivalent Privacy` : encryption technology that provides a very low level of privacy and only uses 40 bits for encryption
- WPA `WiFi Protected Access` : uses 128 bit key
- WPA2 : uses 256 bit key - harder to decrypt
- MAC filtering : user can configure their own access points to only allow for connections from a specific set of MAC addresses belonging to devices they trust

Cellular Networking (Mobile networking)
- operates over radio waves, and there are specific frequency bands reserved for cellular transmission
- these frequencies can travel over longer distance
- Cellular networks are built around the concept of cells, where each cells is assigned with specific frequency band for use and not overlapping with its neighbouring cells
	![]((../image/cellularNetworking.png)

---

### Week 6

ICMP `Internet Control Message Protocol`
- ICMP packet : 
`Type (8 bit) | Code (8 bit) | Checksum (16 bit)`
`Rest of Header`
`Data Section (Payload)`
   - Payload for ICMP packet exists entirely so that the recipient of the message knows which of their transmissions caused the error being reported

> Ping lets user send a speical type of ICMP message called an `Echo Request`. If the destination is up and running and able to communicate on the network, it'll send back an ICMP Echo Reply message type

Traceroute
- Utility that lets us discover the path between 2 nodes, and give information about each hop along the way
- Works through TTL field at IP level; when TTL field reaches zero, the packet is discarded and an ICMP `Time Exceeded` message is sent back to the originating host
![]((../image/traceroute.png)

More on DNS 

- `nslookup` : output displays what server was used to perform the request and the resolution result (i.e. `nslookup twitter` and it will return twitter's server & address)
- The IP addresses for Level 3s public DNS servers: from 4.2.2.1 to 4.2.2.6.
- Google operates public DNS server at `8.8.8.8` `8.8.4.4`
- Most public DNS servers are available globally through anycast

> Always make sure the Name SErver is run by a reputable company, and try to use the name servers provided by your ISP outside of troubleshooting scenarios

- Hosts File : flat file that contains a network address followed by the host name it can be referred to as
	- i.e. 1.2.3.4 webserver
    - Loopback address : sending network traffic to yourself
    - The loop back IP for IPV 4 is `127.0.0.1`
    - The loop back IP for IPV 6 is `127.0.0.1::1`
    - Host files are examined before a DNS resolution attempt occurs on just about every major operating system.

#### Cloud

**Cloud Computing**: a technological approach where computing resources are provisioned in a shareable way, so that lots of users get what they need when they need it; New model in computing where large clusters of machines let us use the total resources available in a better way
- Hardware Virtualization(= single physical machine, called a host could run many individual virtual instances, called guests
- Hypervisor : SW that runs and manages virtual machines, while also offering these guests a virtual operating platform that's indistinguishable from actual hardware
	![]((../image/hw-virtualization.png)
- Public Cloud
- Private Cloud
- Hybrid Cloud (mix of public & Cloud

>Everything-as-a-Service
1. Infrastructure-aaS : You shouldn;t have to worry about building your own network or your own servers
2. Platform-aaS : Subset of cloud computing where a platform is provided for customers to run their services
3. Software-aaS : Way of licensing the use of SW to others whlie keeping that SW centrally hosted and managed (i.e. Gmail for businesss, Office 365 Outlook)

Cloud Storage : customer contracts a cloud storage provider to keep their data secure, accessible, and available
- provides protection against data loss
- Cloud storage solutions also grow with user. User needs to pay for exactly how much storage they used instead of having a fixed amount (like local storage)

#### IPv6 

IPv6 Addressing and Subnetting
- 128 bit in size; $2^{128}$ = 39 digit long number (_Undecillion_)
- 8 groups of 16 bits each: `2001:0db8:0000:0000:0000:ff00:0012:3456`
- First 2 groups`2001:0db8` is reserved for documentation, education, books, courses
- Two rules of shortening IPv6 address
	1. Remove any leading 0s
    2. Any number of consecutive groups composed of just 0s can be replaced with two colons
    	- So this `2001:0db8:0000:0000:0000:ff00:0012:3456`
        - will look like `2001:db8::ff00:12:3456`
- IPv6 loopback address `::1`
- `ff00` - reserved for mulicast
- `fe80` reserved for link-local unicast : allow for local network segment communications and are configures based upon host's MAC address
- First half of IPv6 is Network ID, second half of IPv6 is for Host ID

IPv6 Headers
1. Version field `4 bit` Defines what version of IP is in use
2. Traffic class field `8 bit` Defines the type of traffic contained within the IP datagram, and allows for different classes of traffic to receive different priorities
3. Flow Label field `20 bit` Used in conjunction with the traffic class field foe routers to make decisions about the quality of service level foe a specific datagram
4. Payload length field `16 bit` Defines how long the data payload section of the datagram is
5. Next Header field (unique in IPv6; optional)
6. Hop limit field `8 bit` Identical purpose as TTL field in IPv4 
7. Source Address `128 bit`
8. Destination Address `128 bit`

IPv6 & IPv4
- IPv4 mapped address space :  Any IPv6 address that begins with 80 zeros, and is then followed by 16 ones is understood to be part of the IPv4 mapped address space
	`192.168.1.1 = 0:0:0:0:0:ffff:d1ad:35a7`
- IPv6 Tunnels : Servers take incoming IPv6 traffic and encapsulate it within traditional IPv4 datagram
	![]((../image/ipv6-tunneling.png)
    - IPv6 tunnel broker : companies that provide IPv6 tunneling endpoints for us, so we don't have to introduce additional equipment to our network


