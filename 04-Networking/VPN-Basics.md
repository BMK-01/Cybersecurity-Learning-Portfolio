# VPN Basics

## Overview
A Virtual Private Network (VPN) is a technology that allows devices on separate networks to communicate securely by creating a dedicated path between each other over the Internet (known as a tunnel). 
Devices connected within this tunnel form their own private network.

## Security Relevance
VPNs are critical in cybersecurity because they protect data in transit from eavesdropping and Man-in-the-Middle (MitM) attacks. 
Organizations heavily rely on VPNs to allow remote workers secure access to internal corporate networks without exposing those sensitive internal systems to the public internet.
Furthermore, since every attack and defense travels across a network first, 
defenders must understand VPNs because attackers frequently use them to mask their true geographical locations and bypass network filters.

## What I Learned (Learning Objectives)
### Benefits of VPN
- **Allows networks in different geographical locations to be connected:** For example, a business with multiple offices will find VPNs beneficial,
as it means that resources like servers/infrastructure can be accessed from another office.
- **Offers privacy:** VPN technology uses encryption to protect data. This means that it can only be understood between the devices it was being sent from and is destined for,
meaning the data isn't vulnerable to sniffing.
- **Offers anonymity:** Usually, your traffic can be viewed by your ISP and other intermediaries and, therefore, tracked. 
The level of anonymity a VPN provides is only as much as how other devices on the network respect privacy.
For example, a VPN that logs all of your data/history is essentially the same as not using a VPN in this regard.

### VPN Technologies
- **PPP**
This technology is used by PPTP (explained below) to allow for authentication and provide encryption of data. VPNs work by using a private key and public certificate (similar to SSH).
A private key & certificate must match for you to connect. This technology is not capable of leaving a network by itself (non-routable).
- **PPTP**
The Point-to-Point Tunneling Protocol (PPTP) is the technology that allows the data from PPP to travel and leave a network. 
PPTP is very easy to set up and is supported by most devices. It is, however, weakly encrypted in comparison to alternatives.
- **IPSec**
Internet Protocol Security (IPsec) encrypts data using the existing Internet Protocol (IP) framework.
IPSec is difficult to set up in comparison to alternatives; however, if successful, it boasts strong encryption and is also supported on many devices.


## What I Practiced (Hands-on labs)
I've always used VPNs, whether it was to connect to my patreon account or access Netflix shows that weren't available in my region so I definetely am not new to using it.

## New Terms / Key Concepts
- VPN
- Tunnel
- PPP
- PPTP
- IPSec
 
## Sources
- [TryHackMe — Extending Your Network (Room)](https://tryhackme.com/room/extendingyournetwork?taskNo=4&sharerId=68c953756987851d0822866a)
- [YouTube — Network Direction's Video](https://youtube.com/playlist?list=PLDQaRcbiSnqF5U8ffMgZzS7fq1rHUI3Q8&si=ZgAUsMQuCi-huXD7)
- Online Articles 
