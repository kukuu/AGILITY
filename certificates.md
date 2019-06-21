# Certificates & Digital Security

Server Certificates -  Are basically used to identify a server. ... Whereas client certificates as the name implies are clearly used to identify a client to a respective user, which means authenticating the client to the server. Both SSL certificate (server) and client certificate encompass the “Issued to” section

PKI - A public key infrastructure (PKI) is a set of rules, policies, and procedures needed to create, manage, distribute, use, store, and revoke digital certificates and manage public-key encryption. In a Microsoft PKI, a registration authority is usually called a subordinate CA.

A secure server certificate (not to be confused with a personal certificate) -  Is a digital certificate issued to a Web server by a trusted certification service known as a Certificate Authority (CA). Transactions between the server and client are encrypted.


## SSL
SSL Certificates - Are small data files that digitally bind a cryptographic key to an organization's details. When installed on a web server, it activates the padlock and the https protocol and allows secure connections from a web server to a browser.

Typically, SSL is used to secure credit card transactions, data transfer and logins, and more recently is becoming the norm when securing browsing of social media sites.

SSL (Secure Socket Layer - 1995  e.g. POODLE, DROWN)  Certificates bind together:

1. A domain name, server name or hostname.

2. An organizational identity (i.e. company name) and location.

An organization needs to install the SSL Certificate onto its web server to initiate a secure session with browsers. Once a secure connection is established, all web traffic between the web server and the web browser will be secure.

When a certificate is successfully installed on your server, the application protocol (also known as HTTP) will change to HTTPs, where the ‘S’ stands for ‘secure’. Depending on the type of certificate you purchase and what browser you are surfing the internet on, a browser will show a padlock or green bar in the browser when you visit a website that has an SSL Certificate installed.

## TLS

TLS was introduced in 1999 as a new version of SSL and was based on SSL 3.0: Transport Layer Security (TLS) is just a new name for SSL v4 - essentially, we are talking about the same protocol.

It’s worth noting here that SSL and TLS simply refer to the handshake that takes place between a client and a server. The handshake doesn’t actually do any encryption itself, it just agrees on a shared secret and type of encryption that is going to be used.

## Encryption

https://github.com/kukuu/AGILITY/blob/master/white-paper/security-encryption.md 

##  Blockchain

It is a decentralised platform and peer to peer avoiding hacking.

By storing data across its network, the blockchain eliminates the risks that come with data being held centrally.

Its network lacks centralized points of vulnerability that computer hackers can exploit. Today’s internet has security problems that are familiar to everyone. We all rely on the “username/password” system to protect our identity and assets online. Blockchain security methods use encryption technology.

With Blockchain Users to the network have private keys and the network stores public keys for encryption/decryption when called upon.

### Ethereum 

https://blockgeeks.com/guides/ethereum/

## JWT 

    https://github.com/kukuu/AGILITY/blob/master/white-paper/JWT-architecture.png

## OAuth

https://github.com/kukuu/-SECURE-API


## 2FA

https://github.com/kukuu/worldlabs/tree/master/KF-NFT/Authy-2FA


## SAML



## OAuth 2

# Resources 

1. Cloud Native Security - https://www.twistlock.com/2017/10/02/security-cloud-native-environments/?ads_cmpid=1071572634&ads_adid=54488335919&ads_matchtype=b&ads_network=g&ads_creative=269316971720&utm_term=&ads_targetid=dsa-446131505180&utm_campaign=&utm_source=adwords&utm_medium=ppc&ttv=2&gclid=EAIaIQobChMIld3mtZqF3QIVqrXtCh16MwdBEAAYAyAAEgLSO_D_BwE
