# TCP/IP (The Three Way Handshake)

## Overview
Transmission Control Protocol (TCP) is a connection-oriented network protocol that guarantees the reliable, ordered delivery of data between machines. 
Before sending any actual information, it establishes a strict connection using a "three-way handshake" to ensure that no data packets are lost, delayed, or corrupted in transit.

## Security Relevance
Understanding the TCP three-way handshake is crucial in cybersecurity because attackers actively exploit this specific connection mechanism. 
Adversaries launch Denial of Service (DoS) attacks, such as SYN floods, by initiating handshakes but never completing the final step, leaving connections half-open to exhaust and crash server resources. 
Defenders must know exactly how this protocol behaves to configure firewall rules, analyze packet captures, and trace malicious requests across the network.

## What I Learned (Learning Objectives)
The TCP/IP protocol consists of four layers and is arguably just a summarised version of the OSI model. These layers are:
- Application
- Transport
- Internet
- Network Interface

Very similar to how the OSI model works, information is added to each layer of the TCP model as the piece of data (or packet) traverses it. This process is known as encapsulation - where the reverse of this process is decapsulation.

| Advantages of TCP | Disadvantages of TCP |
|----------|----------|
| Guarantees the integrity of data. | Requires a reliable connection between the two devices. If one small chunk of data is not received, then the entire chunk of data cannot be used and must be re-sent.|
| Capable of synchronising two devices to prevent each other from being flooded with data in the wrong order. | A slow connection can bottleneck another device as the connection will be reserved on the other device the whole time.  |
| Performs a lot more processes for reliability. | TCP is significantly slower than UDP because more work (computing) has to be done by the devices using this protocol. |


## What I Practiced (Hands-on labs)
On TryHackMe's Lab Machine, I helped two machine's communicate by re-assembling the TCP handshake in the correct order in the static lab attached to the task.

## New Terms / Key Concepts
- TCP/IP
- Three-Way Handshake
- Encapsulation & Decapsulation
- Integrity
- Source and Destination Port
- Source and Destination IP
- Sequence Number (SYN)
- Acknowledgement Number (ACK)
- Checksum
- Data
- Flag

 
## Sources
- [TryHackMe — Packets & Frames (Room)](hhttps://tryhackme.com/room/packetsframes?taskNo=2&sharerId=68c953756987851d0822866a)
- Online Articles 
