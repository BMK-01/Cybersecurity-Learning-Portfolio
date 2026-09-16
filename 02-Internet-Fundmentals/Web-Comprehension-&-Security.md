# Web Comprehension & Security

## Overview
Websites are fundamentally split into two primary components: the back end (server-side) and the front end (client-side). 
A client application, such as a web browser, acts as a translator for the front end. It sends a request to a server, receives raw code (like HTML, CSS, and JavaScript) in return, and renders it into a visual, readable webpage for the user.

## Security Relevance
Because client applications operate at the Application layer, they are a frequent target for exploitation. 
If a website fails to properly sanitize user input, attackers can launch specific Application layer attacks—such as Cross-Site Scripting (XSS) or HTML Injection—to manipulate the page structure or hijack user sessions directly within the browser environment. 
Furthermore, attackers routinely inspect a webpage's rendered source code to exploit Sensitive Data Exposure, searching for hidden developer comments or hardcoded credentials left behind in the clear text.

## What I Learned (Learning Objectives)
* **HTML (HyperText Markup Language):** Learned that HTML provides the foundational structure of a page using specific elements (tags) like `<h1>`, `<p>`, and `<img>`.
* **JavaScript (JS):** Discovered that while HTML is static, JavaScript is the programming language that allows web pages to become dynamic and interactive (e.g., updating content without a full page reload).
* **Front End vs. Back End:** Solidified the distinction between the remote server that processes data and the local client browser that renders it.
* **Sensitive Data Exposure:** Recognized the security risks of leaving sensitive information, such as passwords, in client-side HTML comments where any user can simply right-click and select "View Page Source" to see it.
* **HTML Injection:** Understood that unsanitized input fields can be weaponized by an attacker to inject arbitrary HTML code (like malicious anchor links) into the webpage's structure.

## What I Practiced (Hands-on labs)
* Inspected the provided HTML code and fixed a broken `<img>` tag by appending the missing `.jpg` extension to reveal the hidden flag `HTMLHERO`.
* Injected a new `<img>` tag into the editor, pointing to `img/dog-1.png`, which rendered a picture and outputted the flag `DOGHTML`.
* Utilized the site editor to add custom JavaScript (`document.getElementById("demo").innerHTML = "Hack the Planet"`) to dynamically change page content and capture the `JSISFUN` flag.
* Analyzed the page source of a simulated target webpage and located a hidden multi-line HTML comment containing the exposed password `testpasswd`.
* Executed an HTML Injection attack by inserting an anchor tag (`<a href="[http://hacker.com](http://hacker.com)">malicious</a>`) into an unsanitized input field to trigger the `HTML_INJ3CTI0N` flag.

## New Terms / Key Concepts
* Front End & Back End
* HTML (HyperText Markup Language)
* CSS (Cascading Style Sheets)
* JavaScript (JS)
* DOM (Document Object Model)
* Sensitive Data Exposure
* HTML Injection

## Sources
- [TryHackMe — How Websites Work (Room)](https://tryhackme.com/room/howwebsiteswork?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=68c953756987851d0822866a)
- Online Articles
