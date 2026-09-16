# HTTP

## Overview
HyperText Transfer Protocol (HTTP) is the foundational protocol used for communication between web browsers and web servers. Developed by Tim Berners-Lee, it dictates how data is formatted and transmitted across the internet. HTTPS is the secure, encrypted version of this protocol, providing assurances that data is safe from interception and that the client is communicating with the correct, legitimate web server.

## Security Relevance
Because standard HTTP is a plaintext protocol, any data transmitted—such as passwords or session cookies—can be easily intercepted and read by an attacker on the same network. HTTPS mitigates this by encrypting the traffic. Furthermore, a deep understanding of HTTP methods, headers, and status codes is essential in cybersecurity; attackers frequently manipulate these components (e.g., exploiting insecure `PUT` methods or modifying headers) to test web application logic, bypass access controls, or execute attacks like Cross-Site Scripting (XSS).

## What I Learned (Learning Objectives)
* **Requests & Responses:** Examined how a client sends a structured request (including the protocol version like HTTP/1.1) and how servers return a response with specific headers, such as `Content-Length`, to indicate how much data to expect.
* **URL Structure:** Broke down Uniform Resource Locators (URLs) into their core components: Scheme, User (authentication), Host, Port, Path, Query String, and Fragment.
* **HTTP Methods (GET / POST):** Learned that `GET` is used to retrieve information (like viewing a web page) while `POST` is used to submit new data (like creating a user account).
* **HTTP Methods (PUT / DELETE):** Learned that `PUT` is used to update existing data (like changing an email address) and `DELETE` is used to remove information (like deleting a profile picture).
* **HTTP Status Codes:** Explored the five ranges of status codes (100s to 500s) and identified common codes such as `201 Created`, `401 Not Authorised`, `404 Page Not Found`, and `503 Service Unavailable`.
* **Headers & Cookies:** Learned how headers like `User-Agent` identify browser software, `Content-Type` dictates the data format, and `Set-Cookie` manages stateful user authentication over a stateless protocol.

## What I Practiced (Hands-on labs)
* Investigated a mock webpage to identify a missing SSL/TLS certificate, uncovering the flag `THM{INVALID_HTTP_CERT}`.
* Utilized a split-screen interactive simulator to manually construct and send a `GET` request to the `/room` path, retrieving the flag `THM{YOU'RE_IN_THE_ROOM}`.
* Executed a `GET` request to `/blog` while configuring URI parameters using the gear icon to set `id=1`, obtaining `THM{YOU_FOUND_THE_BLOG}`.
* Constructed a `DELETE` request to `/user/1`, resulting in the flag `THM{USER_IS_DELETED}`.
* Sent a `PUT` request to `/user/2` and modified the body parameters to set the username to `admin`, capturing `THM{USER_HAS_UPDATED}`.
* Dispatched a `POST` request to `/login` with the body parameters `username` set to `thm` and `password` set to `letmein`.

## New Terms / Key Concepts
* HTTP / HTTPS
* URL (Uniform Resource Locator)
* HTTP Methods (GET, POST, PUT, DELETE)
* Status Codes (1xx - 5xx)
* Headers (`User-Agent`, `Host`, `Content-Length`, `Content-Type`)
* Cookies (`Set-Cookie`)
* Query String & URI Parameters

## Sources
- [TryHackMe — HTTP In Detail (Room)](https://tryhackme.com/room/httpindetail?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles
