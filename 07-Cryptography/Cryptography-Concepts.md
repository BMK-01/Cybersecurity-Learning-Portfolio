# Cryptography Concepts

## Overview
Cryptography is the practice of using mathematical rules and secret keys to scramble readable data (plaintext) into gibberish (ciphertext) to protect it from unauthorized access. 
This discipline ensures that information can travel safely across public networks, like the internet, by relying on public algorithms combined with closely guarded secret keys to secure the data in transit.

## Security Relevance
Cryptography forms the backbone of digital security, directly supporting the core pillars of the CIA Triad (Confidentiality, Integrity, and Availability). 
As established in Phase 6, cryptography is a fundamental mechanism used to defend systems you already understand. Without it, any intercepted data would be exposed to unauthorized disclosure or alteration. 
By utilizing both symmetric and asymmetric encryption, security professionals protect sensitive communications, verify digital identities, and secure web traffic against interception by threat actors.

## What I Learned (Learning Objectives)
* **Encryption Core Principles:** Learned that security relies on keeping keys secret rather than hiding the algorithm itself, which is typically public and heavily tested.
* **Plaintext vs. Ciphertext:** Solidified the difference between the readable original message (plaintext) and the scrambled, unreadable output (ciphertext).
* **Symmetric Encryption:** Discovered that symmetric encryption uses a single shared key to both lock (encrypt) and unlock (decrypt) a message, requiring a highly secure way to distribute that key.
* **Asymmetric Encryption:** Understood that asymmetric encryption utilizes a mathematically linked key pair: a public key used to encrypt the data, and a private key that must remain safely kept to decrypt it.
* **Hybrid Systems:** Explored how modern protocols like HTTPS use asymmetric encryption for the initial secure key exchange and then switch to symmetric encryption for faster bulk data transfer.

## What I Practiced (Hands-on labs)
* Completed the interactive Secret Message Rescue game to encrypt and decrypt messages using varying shift keys, capturing the completion flag.
* Utilized the Caesar cipher with a shift key of 3 to manually decode the ciphertext `DWWDFN WRPRUURZ` back into the plaintext `ATTACK TOMORROW`.
* Encrypted the word `CYBER` into `HDGJW` using a Caesar cipher shift key of 5 to simulate the symmetric encryption process.
* Identified the weakness of limited key spaces by brute-forcing the ciphertext `ESP DJDEPX TD LE CTDV` to find the correct shift key of 11, revealing `THE SYSTEM IS AT RISK`.
* Decoded the ROT13 ciphertext `FVZCYR PNRFNE PVCURE` by shifting the alphabet by 13 spaces to uncover the hidden `SIMPLE CAESAR CIPHER` message.

## New Terms / Key Concepts
* Plaintext
* Ciphertext
* Symmetric Encryption
* Asymmetric Encryption
* Public & Private Keys
* Algorithm
* Caesar Cipher & ROT13

## Sources
- [TryHackMe — Cryptography Concepts (Room)](https://tryhackme.com/room/cryptographyconcepts?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles
