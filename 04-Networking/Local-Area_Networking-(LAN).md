# LAN (Local Area Networking)

## Overview
A Local Area Network (LAN) is a network that interconnects computers and devices within a limited geographical area, such as a home, school, or office building. 
It enables physical devices on the same local network segment to share resources, transfer data rapidly, and route traffic to external gateways.

## Security Relevance
LAN security is critical in cybersecurity because once an attacker gains access to a local network, they can bypass perimeter defenses and target other local devices. 
Adversaries often execute local network attacks, such as ARP spoofing or MAC address spoofing—to intercept local traffic, perform Man-in-the-Middle (MitM) attacks, or move laterally across the network.

## What I Learned (Learning Objectives)
### Local Area Network (LAN) Topologies
In reference to networking, the term "topology" refers to the design or look of the network at hand.
- **Star Topology:** The main premise of a star topology is that devices are individually connected via a central networking device such as a switch or hub.
  This topology is the most commonly found today because of its reliability and scalability - despite the cost.
- **Bus Topology:** This type of connection relies upon a single connection which is known as a backbone cable.
  This type of topology is similar to the leaf off of a tree in the sense that devices (leaves) stem from where the branches are on this cable.
- **Ring topology:** (also known as token topology) boasts some similarities. Devices such as computers are connected directly to each other to form a loop,
meaning that there is little cabling required and less dependence on dedicated hardware such as within a star topology.

### Switch
Switches are dedicated devices within a network that are designed to aggregate multiple other devices such as computers, printers, or any other networking-capable device using ethernet.
These various devices plug into a switch's port. Switches are usually found in larger networks such as businesses, schools, or similar-sized networks, where there are many devices to connect to the network.

### Router
Is a device who's job is to connect networks and pass data between them. It does this by using routing (hence the name router!).
Routing is the label given to the process of data travelling across networks.

### Subnetting
Subnetting is the term given to splitting up a network into smaller, miniature networks within itself.
Subnetting is achieved by splitting up the number of hosts that can fit within the network, represented by a number called a subnet mask. 
It provides a range of benefits, including: efficiency, security, full control etc.

Subnets use IP addresses in three different ways:
- **Identify the network address:** This address identifies the start of the actual network and is used to identify a network's existence.
- **Identify the host address:** An IP address here is used to identify a device on the subnet.
- **Identify the default gateway:** The default gateway address is a special address assigned to a device on the network that is capable of sending information to another network. 

### Address Resolution Protocol (ARP) 
Is responsible for finding the MAC (hardware) address related to a specific IP address. 
It works by broadcasting an ARP query, "Who has this IP address? Tell me." And the response is of the form, "The IP address is at this MAC address."

### Dynamic Host Configuration Protocol (DHCP) 
Is a network management protocol used on Internet Protocol (IP) networksfor automatically assigning IP addresses and other communication parameters to devices connected to the network using a client–server architecture.

When a device connects to a network, if it has not already been manually assigned an IP address, it sends out a request (DHCP Discover) to see if any DHCP servers are on the network. 
The DHCP server then replies back with an IP address the device could use (DHCP Offer). 
The device then sends a reply confirming it wants the offered IP Address (DHCP Request), 
lastly, the DHCP server sends a reply acknowledging this has been completed, and the device can start using the IP Address (DHCP ACK).



## What I Practiced (Hands-on labs)
On TryHackMe's Interactive Lab Machine, I practically learnt about the various ways in which LAN topologies are vulnerable to breaking. 
I Broke all three LAN topologies to retrieve a flag.

## New Terms / Key Concepts
- Lan Topologies
- Mac Address
- Ip Address
- Router
- Switch
- Subnetting
- ARP
- DHCP

 
## Sources
- [TryHackMe — Intro to LAN Room](https://tryhackme.com/room/introtolan?utm_campaign=social_share&utm_medium=social&utm_content=room&utm_source=copy&sharerId=68c953756987851d0822866a)
- [Youtube — Network Direction Channel]()
- Online Articles 
