# Firewalls 101

## Overview
A firewall is a device within a network responsible for determining what traffic is allowed to enter and exit. 
Think of a firewall as border security for a network that stops unauthorized incoming and outgoing traffic. 

## Security Relevance
Firewalls are a critical first line of defense in cybersecurity because they prevent unauthorized access to internal systems. 
Defenders configure specific firewall rules based on protocols like TCP and UDP to filter traffic and spot anomalies.

## What I Learned (Learning Objectives)
### Firewall Configuration
An administrator can configure a firewall to permit or deny traffic from entering or exiting a network based on numerous factors such as:
- Where the traffic is coming from? (has the firewall been told to accept/deny traffic from a specific network?)
- Where is the traffic going to? ('' destined for a specific network?)
- What port is the traffic for? ('' destined for port 80 only?)
- What protocol is the traffic using? ('' that is UDP, TCP or both?)

### Firewall Categories
Firewalls come in all shapes and sizes. 
From dedicated pieces of hardware (often found in large networks like businesses) that can handle a magnitude of data to residential routers (like at a home) or software such as Snort, 
firewalls can be categorised into 2 to 5 categories. 

The two primary categories of firewalls are:
- **Stateful:** This type of firewall uses the entire information from a connection;
rather than inspecting an individual packet, this firewall determines the behaviour of a device based upon the entire connection.

- **Stateless:**
This firewall type uses a static set of rules to determine whether or not individual packets are acceptable or not.
For example, a device sending a bad packet will not necessarily mean that the entire device is then blocked.

## What I Practiced (Hands-on labs)
On TryHackMe's Lab Machine, Malicious traffic were heading to a webserver through port 80. 
I Configured a firewall to prevent the malicious packets from reaching the web sever allowing only the legitimate traffic pass through.

## New Terms / Key Concepts
- Port forwarding
- Traffic
- Intranet
- Stateful
- Stateless
- Distributed Denial-of-Service attack

## Sources
- [TryHackMe — Extending Your Network (Room)](https://tryhackme.com/room/extendingyournetwork?taskNo=2&sharerId=68c953756987851d0822866a)
- [YouTube — Network Direction's Video](https://youtube.com/playlist?list=PLDQaRcbiSnqF5U8ffMgZzS7fq1rHUI3Q8&si=ZgAUsMQuCi-huXD7)
- Online Articles 
