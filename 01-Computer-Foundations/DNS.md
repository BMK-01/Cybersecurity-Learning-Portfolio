# Domain Name System (DNS)

## Overview
The Domain Name System (DNS) acts as the internet's phonebook, translating human-friendly domain names (like google.com) into the numerical IP addresses that computers need to locate each other and route traffic. It bridges the gap between how humans remember websites and how machines actually talk to each other across a network for name resolution.

## Security Relevance
DNS is a frequent target in cybersecurity because if an attacker controls where a name resolves, they control the destination of the traffic. Adversaries use attacks like DNS spoofing or cache poisoning to secretly redirect a user's legitimate request for a secure site to a malicious, fake clone to steal credentials. Additionally, malware often uses a technique called DNS tunneling to sneak stolen data out of a corporate network without triggering standard firewall rules

## What I Learned (Learning Objectives)
 * **Domain Hierarchy:** Domains are structured starting from the Root Domain down to Top-Level Domains (TLDs) and Second-Level Domains.
 * **Domain Limitations:** A Second-Level Domain or subdomain is limited to 63 characters, must use specific alphanumeric formatting, and cannot start or end with hyphens.
 * **DNS Record Types:** Multiple types of DNS records exist, including A records for IPv4, AAAA records for IPv6, and CNAME records that resolve to another domain name.
 * **Email and Verification Records:** MX records resolve to the servers that handle email for a domain, while TXT records are free text fields often used to list servers with the authority to send emails.
 * **Request Lifecycle:** Traced how a query checks a local cache before progressing to recursive servers (usually provided by an ISP), root servers, TLD servers, and authoritative servers.
 * **Time To Live (TTL):** Discovered that the TTL field dictates exactly how long a DNS record should be cached locally to save on repeat requests.

## What I Practiced (Hands-on labs)
 * Utilized a split-screen simulator to execute nslookup command-line queries against the website.thm domain to uncover various records.
 * Queried the CNAME record for shop.website.thm, which resolved to the alias shops.myshopify.com.
 * Retrieved the TXT record for website.thm to capture a hidden flag: THM{7012BBA60997F35A9516C2E16D2944FF}.
 * Investigated the MX record for website.thm and identified its numerical priority value as 30.
 * Extracted the IPv4 address 10.10.10.10 by performing an A record lookup on www.website.thm.

## New Terms / Key Concepts
 * Domain
 * IP Address
 * Domain Hierarchy
 * Subdomain
 * nslookup
 * Time To Live (TTL)
 * Recursive & Authoritative Servers

## Sources
- [TryHackMe — DNS In Detail (Room)](https://tryhackme.com/room/dnsindetail?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles
