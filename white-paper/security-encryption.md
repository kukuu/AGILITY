# Security and Encryption

Symmetric encryption uses a single key that needs to be shared among the people who need to receive the message while asymmetrical encryption uses a pair of public key and a private key to encrypt and decrypt messages when communicating. Asymmetric encryption takes relatively more time than the symmetric encryption.

## Symmetric Encryption
Symmetric encryption is a conventional method of Encryption. It is also the simplest of two techniques. Symmetric encryption is executed by means of only one secret key known as ‘Symmetric Key’ that is possessed by both parties. This key is applied to encode and decode the information. The sender uses this key before sending the message and the receiver uses it to decipher the encoded message.

This is a pretty straightforward technique and as a result, it doesn’t take much time. When it comes to transferring huge data, symmetrical keys are preferred. Caesar’s Cipher happens to be a good example of symmetric encryption. Modern approaches of symmetric encryption are executed using algorithms such as RC4, AES, DES, 3DES, QUAD, Blowfish etc.

The most common form of symmetric encryption comes once an encrypted connection has been negotiated between a client and a server with an SSL certificate installed. Once the connection is negotiated, two 256-bit session keys are created and exchanged so that encrypted communication can occur.

### Core  sticking features:

i. Number of Cryptographic Keys: Symmetric encryption incorporates only one key for encryption as well as decryption.

ii. Complexity:	Symmetric encryption is a simple technique compared to asymmetric encryption as only one key is employed to carry out both the operations.

iii. Swiftness of Execution:	Due to its simplistic nature, both the operations can be carried out pretty quickly.

```
AES -  The Advanced Encryption Standard is actually commonly paired with RSA as its symmetric partner. 
DES
3DES
QUAD
RC4

```


## Asymmetric Encryption

Asymmetric Encryption is a relatively new and complex mode of Encryption. Complex because it incorporates two cryptographic keys to implement data security. These keys are called a Public Key and a Private Key. The Public key, as the name suggests, is available to everyone who wishes to send a message. On the other hand, the private key is kept at a secure place by the owner of the public key.

The public key encrypts the information to be sent. It uses a specific algorithm in doing so. Whereas, the private key, which is in possession of the receiver, decrypts it. The Same algorithm is behind both these processes.

The involvement of two keys makes Asymmetric Encryption a complex technique. Thus, it proves to be massively beneficial in terms of data security. Diffie-Hellman and RSA algorithm are the most widely used algorithms for Asymmetric Encryption.


### Core sticking features:

i. Number of Cryptographic Keys: Asymmetric Encryption consists of two cryptographic keys. These keys are regarded as Public Key and Private Key. 

ii. Contribution from separate keys for encryption and decryption makes it a rather complex process.

iii. Swiftness of Execution: Because of encryption and decryption by two separate keys and the process of comparing them make it a tad slow procedure.

```

RSA - Rivest-Shamir-Adleman encryption algorithm is one of the most powerful forms of 
encryption in the world

Diffie-Hellman

ECC

El Gamal

DSA

```


## OWASP (Open Web Application Security Project )

OWASP (Open Web Application Security Project) is an organization that provides unbiased and practical, cost-effective information about computer and Internet applications.


The OWASP Top 10 list consists of the 10 most seen application vulnerabilities:

1. Injection.

2. Broken Authentication.

3. Broken Access control.

4. Sensitive data exposure.

5. XML External Entities (XXE)

6. Security misconfigurations.

7. Cross Site Scripting (XSS)

8. Insecure Deserialization.

## Types of injection Attacks

https://dzone.com/articles/what-are-injection-attacks

i. XSS (Cross Site Scripting) - Inject arbitrary JS into a legitimate website/application, which is executed in the users browser.

 

ii. CRLF (Carriage Return Line Feed) - Injection of unexpected CRLF.

Injects an unexpected CRLF (Carriage Return and Line Feed) character sequence used to split an HTTP response header and write arbitrary contents to the response body, including Cross-site Scripting (XSS).



iii. Email injection (Mail Command SMTP) - Injects SMTP/IMAP statements into an email server

Potential Impact 

iv Host Header Injection - Abuses the implicit trust of the HTTP host Header to poison passsword re-set functionality.



v LDAP injection - Injects LDAP (Lightweight  Directory Access Protocol) statements to execute arbitrary LDAP commands including granting permissions and modifying contents of an LDAP tree.


vi. SQLi (SQL injection) - Injects SQL commands that can read or modify data from a database. Advanced variations of this attack can be used to write arbitrary files to the server and even execute OS commands which may lead to full system compromise.



vii. XPath injection - Inject data into an application to execute crafted XPath queries which can be used to access unauthorized data and bypass authentication.

 

viii. Code injection - Injects application code which can execute operating system commands as the user running the web application.



vix. CSRF (XSRF)

Cross-Site Request Forgery (CSRF) is an attack that forces an end user to execute unwanted actions on a web application in which they're currently authenticated. CSRF attacks specifically target state-changing requests, not theft of data, since the attacker has no way to see the response to the forged request.

A csrf token is generated for the forms and Must be tied to the user's sessions. It is used to send requests to the server, in which the token validates them. This is one way of protecting against csrf, another would be checking the referrer header.


## What is the difference between XSS and CSRF?

Fundamental difference is that CSRF (Cross-site Request forgery) happens in authenticated sessions when the server trusts the user/browser, while XSS (Cross-Site scripting) doesn't need an authenticated session and can be exploited when the vulnerable website doesn't do the basics of validating or escaping input.

## XSS Attack 

The concept of XSS is to manipulate client-side scripts of a web application to execute in the manner desired by the malicious user. Such a manipulation can embed a script in a page that can be executed every time the page is loaded, or whenever an associated event is performed.

XSS is a web-based attack performed on vulnerable web applications.
In XSS attacks, the victim is the user and not the application.
In XSS attacks, malicious content is delivered to users using JavaScript.

XSS vulnerabilities gives the attackers the capability to inject client-side scripts into the application, for example to re-direct users to malicious websites

It can be used to hi-jack user accounts, spread worms, and Trojans, access browser history and clipboard contents, control the browser remotely, and scan and exploit online appliances and applications.

Example

Cyber criminals exploited a persistent XSS vulnerability in the eBay website to embed malicious JavaScript in legitimate listings, redirecting them to spoofed eBay login paes for phishing user credentials.


Featurs of XSS:


i. XSS is a web-based attack performed on vulnerable web applications.

ii.In XSS attacks, the victim is the user and not the application.

iii. In XSS attacks, malicious content is delivered to users using JavaScript.

https://www.veracode.com/security/xss



Examples:

For example, the attacker could send the victim a misleading email with a link containing malicious JavaScript. If the victim clicks on the link, the HTTP request is initiated from the victim's browser and sent to the vulnerable web application.


## How to Prevent an SQL Injection

The only sure way to prevent SQL Injection attacks is 

i. Input validation and parametrized queries including prepared statements. The application code should never use the input directly. 

ii. The developer must sanitize all input, not only web form inputs such as login forms. 

iii. They must remove potential malicious code elements such as single quotes. 

iv. It is also a good idea to turn off the visibility of database errors on your production sites. Database errors can be used with SQL Injection to gain information about your database.

https://www.acunetix.com/websitesecurity/sql-injection2/



## Working with Cloud Security 

- https://github.com/kukuu/AGILITY/blob/master/Cloud-app-security.md 

## Certificates & Digital Security

- https://github.com/kukuu/AGILITY/blob/master/certificates.md 

## Security Tips to Keep Express from Getting Pwned

- https://nodesource.com/blog/nine-security-tips-to-keep-express-from-getting-pwned/?utm_source=nodeweekly&utm_medium=email
