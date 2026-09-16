# Offensive Security Basics

## Overview
Offensive security involves seeing systems the way an attacker would by scanning, probing, and exploiting them to understand what makes them vulnerable. 
The goal is todevelop fluency in how attackers think to build sharper defensive instincts, rather than aiming for a career change into pentesting.

## Security Relevance
Offensive security concepts are deliberately placed at the end of the learning path because attacks make more sense once you already understand what they are attacking.
By scanning and probing systems, you develop sharper defensive instincts without needing to focus on pentesting as a full-time career.

## What I Learned (Learning Objectives)
* **Offensive Security Mindset:** Learned that ethical hacking involves simulating cyberattacks to identify vulnerabilities before malicious hackers can exploit them.
* **Hidden Directory Discovery:** Explored how to manually test URLs or use automated enumeration tools to uncover exposed, private web pages.
* **Brute-Force Attacks:** Understood the methodology behind brute-forcing login portals by systematically guessing common username and password combinations.
* **Cybersecurity Career Paths:** Differentiated between red team roles like Penetration Testers who conduct simulated attacks, and blue team roles like Security Analysts who monitor systems and mitigate threats.

## What I Practiced (Hands-on labs)
* Conducted manual path testing against a simulated web application to discover hidden directories by appending common terms like `/admin` and `/register` to the URL.
* Utilized the Gobuster automated enumeration tool alongside a wordlist to successfully discover a hidden `/login` web page.
* Executed a brute-force attack on the discovered login portal by systematically testing a list of common credentials.
* Successfully bypassed authentication using the username `admin` and the password `qwerty` to reveal a hidden secret message.

## New Terms / Key Concepts
* Offensive Security
* Ethical Hacking
* Enumeration
* Brute-Force Attack
* Gobuster & Hydra
* Penetration Testing

## Sources
- [TryHackMe —  Become a Hacker (Room)](https://tryhackme.com/room/becomeahacker?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles
