# Web Basics

## 1. HTTPS

#### Overview
HTTPS (HyperText Transfer Protocol Secure) is an extension of HTTP. It is used to secure communication over a computer network within a web browser.

#### How HTTPS Works
1. **Client Hello**: The client sends a request to the server.
2. **Server Hello**: The server responds with its SSL certificate.
3. **Certificate Verification**: The client verifies the server's certificate.
4. **Key Exchange**: Both parties generate a session key.
5. **Secure Communication**: Encrypted communication begins.

#### Example
Here's an example of an HTTPS request:
```http
GET / HTTP/1.1
Host: www.example.com
```

## 2. DNS

#### Overview

DNS (Domain Name System) is a hierarchical system that translates human-friendly domain names (like www.example.com) into IP addresses.

#### How DNS Works 
1. Query: A user types a domain name into their browser.
2. Recursive Resolver: The query is sent to a recursive DNS resolver.
3. Root Name Server: The resolver queries a root name server.
4. TLD Name Server: The root server directs the resolver to a TLD name server.
5. Authoritative Name Server: The TLD server directs the resolver to an authoritative name server, which provides the IP address for the domain.

### Web Security
#### Importance
Web security involves protecting websites and web applications from attacks. This includes securing data transmitted over the internet and ensuring that web applications are free from vulnerabilities.

#### Common Techniques
1. Content Security Policy (CSP): A security measure to prevent XSS and other code injection attacks.
2. HTTPS: Securing data in transit.
3. Regular Security Audits: Regularly checking for vulnerabilities.

## 3. Web Exploitation Techniques

#### SQL Injection (SQLi)
SQL Injection is a code injection technique that might destroy your database. It is one of the most common web hacking techniques.

Example
A simple SQL Injection example:
```sql
SELECT * FROM users WHERE username = 'admin' --' AND password = 'password';
```

#### Cross-Site Scripting (XSS)
XSS allows attackers to inject malicious scripts into content from otherwise trusted websites.

Example
```js
<script>alert('XSS');</script>
```

### PicoCTF Challenges to try out:

1. [SQLiLite](https://play.picoctf.org/practice/challenge/304?category=1&difficulty=1&page=1)
2. [More SQLi](https://play.picoctf.org/practice/challenge/358?category=1&difficulty=1&page=1)
