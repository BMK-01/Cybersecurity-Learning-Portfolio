# Packets, Frames and Ports

## Overview
Packets and frames are small pieces of data that, when forming together, make a larger piece of information or message. 
However, they are two different things in the OSI model. 
A packet is a piece of data from Layer 3 (Network Layer) of the OSI model, containing information such as an IP header and payload. A frame, however, is used at Layer 2 (Data Link) of the OSI model, which, encapsulates the packet and adds additional information such as MAC addresses.

Perhaps aptly titled by their name, ports are an essential point in which data can be exchanged. Think of a harbour and port. Ships wishing to dock at the harbour will have to go to a port compatible with the dimensions and the facilities located on the ship. When the ship lines up, it will connect to a port at the harbour. Take, for instance, that a cruise liner cannot dock at a port made for a fishing vessel and vice versa. A physical example is how a USB-C cable cannot be plugged into a USB-A port.

## Security Relevance
Understanding packets and frames is essential for analyzing network traffic and deploying the correct defenses. Security professionals inspect packets to detect malicious external IP traffic, such as a Layer 3 ping flood. Conversely, they must analyze frames to detect local network attacks, spotting anomalies like adversaries using MAC spoofing to impersonate trusted devices or ARP poisoning to intercept local traffic.

## What I Learned (Learning Objectives)
- This process of sending data is similar to mailing a letter through the post(basically the same thing actually). The envelope is a frame, which, is used to move the contents (in this analogy, the packet) of the envelope to another place. Once the recepient opens the envelop (frame), they will know how to forward the letter (packet) itself.
- This process is called encapsulation which I have previously learnt discussed in the OSI model. At this stage, it's safe to assume that when we are talking about anything IP addresses, we are talking about **packets**. When the encapsulating information is stripped away, we're talking about the **frame** itself.
- Ports enforce what can park and where — if it isn't compatible, it cannot park here. Networking devices also use ports to enforce strict rules when communicating with one another. When a connection has been established (recalling from the OSI model), any data sent or received by a device will be sent through these ports. In computing, ports are a numerical value between 0 and 65535 (65,535).
- Because ports can range from anywhere between 0-65535, there quickly runs the risk of losing track of what application is using what port. For example, by enforcing that any web browser data is sent over port 80, software developers can design a web browser such as Google Chrome or Firefox to interpret the data the same way as one another. While the standard rule for web data is port 80, a few other protocols have been allocated a standard rule. Any port that is within 0 and 1024 (1,024) is known as a common port. Some of these other protocols are:

| Protocol | Port Number | Description |
|----------|----------|----------|
| File Transfer Protocol (FTP) | 21 | This protocol is used by a file-sharing application built on a client-server model, meaning you can download files from a central location. |
| Secure Shell (SSH) | 22 | This protocol is used to securely login to systems via a text-based interface for management. |
| HyperText Transfer Protocol (HTTP) | 80 | This protocol powers the World Wide Web (WWW)! Your browser uses this to download text, images and videos of web pages. |
| HyperText Transfer Protocol Secure (HTTPS)  | 443 | This protocol does the exact same as above; however, securely using encryption. |
| Server Message Block (SMB) | 445 | This protocol is similar to the File Transfer Protocol (FTP); however, as well as files, SMB allows you to share devices like printers. |
| Remote Desktop Protocol (RDP) | 3389 | This protocol is a secure means of logging in to a system using a visual desktop interface (as opposed to the text-based limitations of the SSH protocol). |

## What I Practiced (Hands-on labs)
On TryHackMe's Lab Machine, I passed a Practical Challenge in which i opened the site attached to the task and connected to the IP address "8.8.8.8" on port "1234", and received a flag.

## New Terms / Key Concepts
- Header
- Time to live (TTL)
- Checksum
- Source & Destination Address
- Source & Destination Port
- Port Protocols
  
## Sources
- [TryHackMe — Packets & Frames (Room)](https://tryhackme.com/room/packetsframes?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles 
