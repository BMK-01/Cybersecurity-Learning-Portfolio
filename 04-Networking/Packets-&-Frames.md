# Packets and Frames

## Overview
Packets and frames are small pieces of data that, when forming together, make a larger piece of information or message. 
However, they are two different things in the OSI model. 
A packet is a piece of data from Layer 3 (Network Layer) of the OSI model, containing information such as an IP header and payload. A frame, however, is used at Layer 2 (Data Link) of the OSI model, which, encapsulates the packet and adds additional information such as MAC addresses.

## Security Relevance
Understanding packets and frames is essential for analyzing network traffic and deploying the correct defenses. Security professionals inspect packets to detect malicious external IP traffic, such as a Layer 3 ping flood. Conversely, they must analyze frames to detect local network attacks, spotting anomalies like adversaries using MAC spoofing to impersonate trusted devices or ARP poisoning to intercept local traffic.

## What I Learned (Learning Objectives)

## What I Practiced (Hands-on labs)
On TryHackMe's Lab Machine,

## New Terms / Key Concepts
- Header
- Time to live (TTL)
- Checksum
- Source & Destination Address
- Source & Destination Port
  
## Sources
- [TryHackMe — Packets & Frames (Room)](https://tryhackme.com/room/packetsframes?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles 
