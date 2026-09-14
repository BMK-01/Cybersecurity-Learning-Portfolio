# Domain Name System (DNS)

## Overview
Domain Name System (DNS) is the protocol responsible for resolving hostnames to their respective IP addresses.
DNS provides a simple way for us to communicate with devices on the internet without remembering complex numbers.

## Security Relevance
DNS is a frequent target in cybersecurity because if an attacker controls where a name resolves, they control the destination of the traffic. 
Adversaries use attacks like DNS spoofing or cache poisoning to secretly redirect a user's legitimate request for a secure site to a malicious, fake clone to steal credentials.

## What I Learned (Learning Objectives)
### Domain Hierarchy
Root Domain - Top-Level Domain - Second-Level Domain.
- **Top-Level Domain (TLD)**
A TLD is the most righthand part of a domain name. So, for example, the tryhackme.com TLD is .com.
There are two types of TLD, gTLD (Generic Top Level) and ccTLD (Country Code Top Level Domain).

- **Second-Level Domain**
Taking tryhackme.com as an example, the .com part is the TLD, and tryhackme is the Second Level Domain.
When registering a domain name, the second-level domain is limited to 63 characters + the TLD and can only use a-z 0-9 and hyphens (cannot start or end with hyphens or have consecutive hyphens).

- **Subdomain**
A subdomain sits on the left-hand side of the Second-Level Domain using a period to separate it; for example, in the name admin.tryhackme.com the admin part is the subdomain.

### DNS Record Types
DNS isn't just for websites though, and multiple types of DNS record exist.
A Record
These records resolve to IPv4 addresses, for example 104.26.10.229

AAAA Record
These records resolve to IPv6 addresses, for example 2606:4700:20::681a:be5

CNAME Record
These records resolve to another domain name, for example, TryHackMe's online shop has the subdomain name store.tryhackme.com which returns a CNAME record shops.shopify.com(opens in new tab).
Another DNS request would then be made to shops.shopify.com(opens in new tab) to work out the IP address.

MX Record
These records resolve to the address of the servers that handle the email for the domain the user is querying, for example an MX record response for tryhackme.com would look something like alt1.aspmx.l.google.com(opens in new tab). 
These records also come with a priority flag. 
This tells the client in which order to try the servers, this is perfect for if the main server goes down and email needs to be sent to a backup server.

TXT Record
TXT records are free text fields where any text-based data can be stored. 
TXT records have multiple uses, but some common ones can be to list servers that have the authority to send an email on behalf of the domain (this can help in the battle against spam and spoofed email)


## What I Practiced (Hands-on labs)


## New Terms / Key Concepts
- Domain
- IP Address
- Domain Hierarchy
- Subdomain
- 
 
## Sources
- 
- Online Articles 
