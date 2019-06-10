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

Working with Cloud Security - https://github.com/kukuu/AGILITY/blob/master/Cloud-app-security.md
