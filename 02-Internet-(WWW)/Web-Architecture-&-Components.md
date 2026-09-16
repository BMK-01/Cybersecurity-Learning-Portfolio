# Web Architecture & Components

## Overview
When a user requests a website, a complex end-to-end process occurs behind the scenes to deliver the content. 
This architecture involves multiple components working together, including load balancers distributing traffic, Content Delivery Networks (CDNs) serving static files, databases storing information, and web servers utilizing virtual hosts to manage multiple domains. 
Understanding this full lifecycle—from the initial DNS request to the final rendering of HTML in the browser—is essential to grasping how the modern web functions.

## Security Relevance
Each component in a web architecture stack plays a specific role in an organization's overall security posture. 
Web Application Firewalls (WAFs) sit between incoming web requests and the server to filter out malicious traffic and stop hacking attempts or Denial of Service (DoS) attacks. Load balancers ensure high availability by performing health checks and re-routing traffic if a server is compromised or taken offline.
Additionally, understanding the strict boundary between frontend (client-side) and backend (server-side) code is critical, as sensitive application logic and database queries must remain securely hidden on the backend to prevent exposure and exploitation.

## What I Learned (Learning Objectives)
* **Load Balancers:** Learned how they handle high traffic and ensure availability by distributing requests across multiple servers using algorithms like round-robin or weighted balancing, and conducting periodic health checks to ensure hosts are alive.
* **Content Delivery Networks (CDNs):** Discovered that CDNs speed up client visits and reduce main server load by geographically distributing and hosting static files like images, CSS, and JavaScript.
* **Web Application Firewalls (WAF):** Understood that a WAF is deployed to protect web servers by inspecting incoming traffic and defending against hacking attempts and DoS attacks.
* **Virtual Hosts:** Explored how web server software (like Apache or Nginx) uses virtual hosts to serve multiple distinct websites and domain names from a single machine.
* **Static vs. Dynamic Content:** Differentiated between static content (which remains exactly the same for every user) and dynamic content (which changes based on different requests, user input, or database interactions).
* **Backend Visibility:** Confirmed that clients cannot view backend code (like server-side logic or database queries), as the server only sends the rendered output to the user's browser.

## What I Practiced (Hands-on labs)
* Answered scenario-based questions to identify the correct architectural components for specific use cases, such as deploying a CDN to speed up static file hosting and relying on health checks to monitor server uptime.
* Completed a drag-and-drop interactive puzzle in the split-screen lab to correctly map the end-to-end flow of a website request.
* Successfully ordered the request lifecycle: Browser Request → Local DNS Cache Check → Recursive DNS Server → Root/Authoritative DNS → WAF → Load Balancer → Port 80/443 Connection → GET Request → Database Communication → HTML Rendering.
* Captured the final completion flag from the quiz: `THM{YOU_GOT_THE_ORDER}`.

## New Terms / Key Concepts
* Load Balancer & Health Checks
* Content Delivery Network (CDN)
* Web Application Firewall (WAF)
* Virtual Hosts
* Static vs. Dynamic Content
* Round-Robin / Weighted Balancing

## Sources
- [TryHackMe — Putting It All Together (Room)](https://tryhackme.com/room/puttingitalltogether?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles
