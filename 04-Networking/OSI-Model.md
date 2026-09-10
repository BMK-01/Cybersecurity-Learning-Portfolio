 # OSI Model

## Overview
The OSI model (Open Systems Interconnection Model) is an essential model used in networking. 
This critical model provides a framework dictating how all networked devices will send, receive and interpret data.
It divides network communication into seven distinct layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application.

## Security Relevance
The OSI model is fundamental in cybersecurity because both attacks and defensive controls are categorized by these specific layers. 
Defenders use the OSI model to pinpoint exactly where a vulnerability exists so they can deploy the correct countermeasures.

## What I Learned (Learning Objectives)
### The seven layers of the OSI model
**7. Application**
This familiarity is because the application layer is the layer in which protocols and rules are in place to determine how the user should interact with data sent or received.
Everyday applications such as email clients, browsers, or file server browsing software such as FileZilla provide a friendly, Graphical User Interface (GUI) for users to interact with data sent or received. 
Other protocols include DNS (Domain Name System), which is how website addresses are translated into IP addresses.

**6. Presentation**
This layer acts as a translator for data to and from the application layer (layer 7).
The receiving computer will also understand data sent to a computer in one format destined for in another format.
For example, when you send an email, the other user may have another email client to you, but the contents of the email will still need to display the same.

Security features such as data encryption (like HTTPS when visiting a secure site) occur at this layer.

**5. Session**
Once data has been correctly translated or formatted from the presentation layer (layer 6), 
the session layer (layer 5) will begin to create and maintain the connection to other computer for which the data is destined. 
When a connection is established, a session is created. Whilst this connection is active, so is the session.
Sessions are unique — meaning that data cannot travel over different sessions, but in fact, only across each session instead.

The session layer is also responsible for closing the connection if it hasn't been used in a while or if it is lost. 

**4. Transport**
Layer 4 of the OSI model plays a vital part in transmitting data across a network and can be a little bit difficult to grasp.
When data is sent between devices, it follows one of two different protocols that are decided based upon several factors:

- **TCP (Transmission Control Protocol):** this protocol is a connection-oriented network protocol that guarantees the reliable, ordered delivery of data between devices.
IT reserves a constant connection between the two devices for the amount of time it takes for the data to be sent and received.
TCP encorporates error checking into its design.

- **UDP (User Daragram Protocol):** is a connectionless network protocol that prioritizes speed over reliability.
Any data that gets sent via UDP is sent to the computer whether it gets there or not. There is no synchronisation between the two devices or guarantee.

**3. Network**
The third layer of the OSI model (network layer) is where the magic of routing & re-assembly of data takes place (from these small chunks to the larger chunk).
Firstly, routing simply determines the most optimal path in which these chunks of data should be sent.
Whilst some protocols at this layer determine exactly what is the "optimal" path that data should take to reach a device, 
I only learnt about their existence at this stage of the networking module. 
Briefly, these protocols include OSPF (Open Shortest Path First) and RIP (Routing Information Protocol). 
The factors that decide what route is taken is decided by the following:

- What path is the shortest? I.e. has the least amount of devices that the packet needs to travel across.
- What path is the most reliable? I.e. have packets been lost on that path before?
- Which path has the faster physical connection? I.e. is one path using a copper connection (slower) or a fibre (considerably faster)?

**2. Data Link**
The data link layer focuses on the physical addressing of the transmission. 
It receives a packet from the network layer (including the IP address for the remote computer) and adds in the physical MAC (Media Access Control) address of the receiving endpoint.
Inside every network-enabled computer is a Network Interface Card (NIC) which comes with a unique MAC address to identify it.

**1. Physical**
This layer references the physical components of the hardware used in networking and is the lowest layer. 
Devices use electrical signals to transfer data between each other in a binary numbering system (1's and 0's).


## What I Practiced (Hands-on labs)
On TryHackMe's interactive Lab Machine, i played an OSI game to test my knowledge and I even beat their staff high score.

## New Terms / Key Concepts
- Application
- Presentation
- Session
- Transport
- Network
- Data Link
- Physical
- NIC
- OSPF
- RIP
- TCP
- UDP
 
## Sources
- [TryHackMe — OSI Model Room](https://tryhackme.com/room/osimodelzi?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- [YouTube — Network Direction's Video](https://youtube.com/playlist?list=PLDQaRcbiSnqF5U8ffMgZzS7fq1rHUI3Q8&si=ZgAUsMQuCi-huXD7)
- Online Articles 
