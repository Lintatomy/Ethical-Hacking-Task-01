# Ethical-Hacking-Task-01

Objective


The purpose of this task is to understand the first phase of Ethical Hacking — Reconnaissance
(Information Gathering). Every penetration test begins by collecting publicly available information about a target. In this task,
you will perform passive reconnaissance only, using publicly available sources.

Part A: Target Selection --

Website Name: GitHub

URL: https://github.com

Reason for choosing the target:
 
 GitHub is one of the world's largest software development platforms. It is publicly accessible, widely used by developers, and suitable for learning passive reconnaissance techniques without performing any unauthorized activities.

 Part B: WHOIS Lookup --

 A public WHOIS lookup service 

* Domain Name
* Registrar
* Registration Date
* Expiry Date
* Name Servers
* Domain Status

Screenshort

<img width="992" height="692" alt="WHOIS" src="https://github.com/user-attachments/assets/0cb92008-f5d1-48ef-b99a-b4be25e3f677" />


Part C: DNS Enumeration --

A Record: -
  Maps a domain name to an IPv4 address, allowing browsers to locate and connect to the correct web server quickly.

Screenshot


  <img width="1041" height="358" alt="DNS-A record" src="https://github.com/user-attachments/assets/0e02b542-2cf8-490b-80d2-cd70e1baa0b4" />



MX Record:-
  Specifies the mail server responsible for receiving emails for a domain, ensuring messages are delivered to the correct destination.

  Screenshot

 <img width="1325" height="362" alt="DNS-MX record" src="https://github.com/user-attachments/assets/a667d499-4ffb-4d9e-8805-554c818c9025" />




 NS Record: -
   Identifies the authoritative name servers managing a domain's DNS records, directing queries to the correct DNS servers reliably.

   Screenshot

   <img width="988" height="861" alt="DNS-NS record" src="https://github.com/user-attachments/assets/e6e8758a-1661-4c66-98c5-84c667adaefa" />




TXT Record:-
  Stores text information in DNS, commonly used for email verification, security policies, domain ownership, and authentication purposes.

  Screenshot

  <img width="710" height="897" alt="DNS-TXT record" src="https://github.com/user-attachments/assets/66fbc91d-d55e-4cff-b14f-ee4d5c2b7c24" />




Part D: Website Technology Identification --

Technologies used by the website
web Server-- 

1. Nginx
2. Apache HTTP Server
3. LiteSpeed
4. Next.js
5. OpenResty
6. IIs
7. Express
8. OpenGSE
9. Caddy
10. Tengine

CMS--

1. WordPress
2. Wix
3. Squarespace
4. GoDaddy Website Builder
5. Drupal
6. Joomla
7. Microsoft SharePoint
8. Weebly
9. Jimdo
10. TYPO3 CMS


Programming Languages --

1. PHP
2. Java
3. Typescript
4. Node.js
5. Python
6. Ruby
7. CFML
8. GraphQL
9. Adobe Flash
10. Erlang

JavaScript Framework--

1. React
2. Emotion
3. GSAP
4. Vue.js
5. Next.js
6. React Router
7. Backbone.js
8. RequireJS
9.styled-components
10. Zone.js

CDN--

1. Cloudflare
2. cdnjs
3. jsDelivr
4. Google Cloud CDN
5. Google Hosted Libraries
6. Amazon CloudFront
7. jQuery CDN
8. Amazon S3
9. Unpkg
10. Hostinger CDN



Part E: HTTP Security Headers --




| **HTTP Security Header**         | **Present (Yes/No)** | **Purpose**                                                                                           |
| -------------------------------- | -------------------- | ----------------------------------------------------------------------------------------------------- |
| Content-Security-Policy (CSP)    | Yes                  | Prevents attacks such as Cross-Site Scripting (XSS) by controlling which content sources are allowed. |
| X-Frame-Options                  | Yes                  | Prevents the website from being embedded in frames, protecting against clickjacking attacks.          |
| X-Content-Type-Options           | Yes                  | Stops browsers from MIME type sniffing, reducing the risk of malicious file execution.                |
| Strict-Transport-Security (HSTS) | Yes                  | Forces browsers to use HTTPS, protecting users from downgrade and man-in-the-middle attacks.          |
| Referrer-Policy                  | Yes                  | Controls how much referrer information is shared when users navigate to other websites.               |



Part F: Robots.txt & Sitemap Analysis --


 1. Robots.txt

URL:https://github.com/robots.txt

Does the website have a robots.txt file?
**Yes**

Information Learned:

* GitHub provides a publicly accessible `robots.txt` file.
* It contains instructions for search engine crawlers.
* Some directories and pages are restricted from indexing.
* The file helps search engines crawl the website more efficiently.
* It is not a security mechanism; it only provides crawler guidance.

Screenshot

<img width="1907" height="966" alt="robots" src="https://github.com/user-attachments/assets/b7fafbe0-8ae5-4096-82ca-87ccee6beb6b" />


2. Sitemap.xml

URL: https://github.com/sitemap.xml

Does the website have a sitemap?
**No** 

GitHub does not provide a public sitemap at this URL. Visiting it returns a **404 Not Found** page.

Information Learned:

* No public sitemap is available at the standard location.
* GitHub may use other methods to help search engines discover and index its content.
* The absence of a public sitemap does not affect the normal operation or accessibility of the website.

Screenshot

<img width="935" height="810" alt="sitmap" src="https://github.com/user-attachments/assets/892ff729-8b8a-4980-a3a3-9361ff011cd4" />



Part G: Reconnaissance Report --



GitHub (https://github.com) was selected as the target because it is a widely used public software development platform suitable for passive reconnaissance. WHOIS lookup revealed domain registration details, registrar information, name servers, and domain status. DNS analysis identified A, MX, NS, and TXT records, providing insight into GitHub's network infrastructure and email configuration. Technology fingerprinting showed the use of modern web technologies, including web servers, CDNs, cloud infrastructure, and security mechanisms. HTTP security header analysis confirmed the presence of Content-Security-Policy (CSP), X-Frame-Options, X-Content-Type-Options, Strict-Transport-Security (HSTS), and Referrer-Policy, demonstrating strong protection against common web attacks. The robots.txt file contained crawler directives and referenced a sitemap to improve search engine indexing. Overall, this exercise demonstrated how valuable information can be gathered using passive reconnaissance without interacting with the target system. It emphasized the importance of ethical information gathering, responsible security practices, and understanding publicly available infrastructure before conducting authorized penetration testing.



Detaied  explaining what i learned during the reconnaissance phase  is attached  in the given PDF

(PART G- Reconnaissance Report.pdf)
