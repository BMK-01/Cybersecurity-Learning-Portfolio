# TCP (The Three Way Handshake) & UDP Internet Protocols

## Overview
Transmission Control Protocol (TCP) is a connection-oriented network protocol that guarantees the reliable, ordered delivery of data between machines. 
Before sending any actual information, it establishes a strict connection using a "three-way handshake" to ensure that no data packets are lost, delayed, or corrupted in transit.

User Datagram Protocol (UDP) is a connectionless protocol; UDP does not require a connection to be established. UDP is suitable for protocols that rely on fast queries, such as DNS, and for protocols that prioritise real-time communications, such as audio/video conferencing and broadcast.

## Security Relevance
TCP and UDP are the core protocols carrying traffic, and mastering them is essential because every attack and every defense travels across a network first. Because UDP is connectionless and does not verify the sender's identity, attackers frequently spoof their addresses to launch massive Amplification DDoS attacks. Defenders must understand both protocols to configure firewall rules, analyze packet captures, and trace malicious requests from the moment they leave a machine to the moment a reply comes back.

## What I Learned (Learning Objectives)
- The TCP/IP protocol consists of four layers and is arguably just a summarised version of the OSI model. These layers are:
 * Application
 * Transport
 * Internet
 * Network Interface

Very similar to how the OSI model works, information is added to each layer of the TCP model as the piece of data (or packet) traverses it. This process is known as encapsulation - where the reverse of this process is decapsulation.

| Advantages of TCP | Disadvantages of TCP |
|----------|----------|
| Guarantees the integrity of data. | Requires a reliable connection between the two devices. If one small chunk of data is not received, then the entire chunk of data cannot be used and must be re-sent.|
| Capable of synchronising two devices to prevent each other from being flooded with data in the wrong order. | A slow connection can bottleneck another device as the connection will be reserved on the other device the whole time.  |
| Performs a lot more processes for reliability. | TCP is significantly slower than UDP because more work (computing) has to be done by the devices using this protocol. |

| Advantages of UDP | Disadvantages of UDP |
|----------|----------|
| UDP is much faster than TCP. | UDP doesn't care if the data is received or not.|
| UDP leaves the application (user software) to decide if there is any control over how quickly packets are sent. | It is quite flexible to software developers in this sense. |
| UDP does not reserve a continuous connection on a device as TCP does. | This means that unstable connections result in a terrible experience for the user. |

## What I Practiced (Hands-on labs)
On TryHackMe's Lab Machine, I helped two machine's communicate by re-assembling the TCP handshake in the correct order in the static lab attached to the task.

## New Terms / Key Concepts
- TCP/IP
- Three-Way Handshake
- Headers
- Encapsulation & Decapsulation
- Integrity
- Source and Destination Port
- Source and Destination IP
- Source and Destination Address
- Sequence Number (SYN)
- Acknowledgement Number (ACK)
- Checksum
- Data
- Flag

 
## Sources
- [TryHackMe — Packets & Frames (Room)](https://tryhackme.com/room/packetsframes?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles 
