# encryption
---
Topics:
Status: #inboxnote
Created: 2022-07-17 17:04:37

---

It allows us to convert normal data to what is essentially unreadable using different math algorithms.

It can protect
- data at rest: Inactive data e.g. on a file
- data in transit: Data in memory on the network
- data in use: Data undergoing current changes

We use a hybrid implementation to get benefits of both

## Symmetric

When we can use the same key to encrypt and decrpyt the message

We need to worry about the distribution of keys but these algorithms tend to be significantly faster

Common algorithms are
- [[DES]]
- [[3DES]]
- [[IDEA]]
- [[AES]]
- [[Blowfish]]
- [[Twofish]]
- [[RC]]

## Asymmetric

This uses a private and public key. Each key can only encrypt or decrypt the data

## Stream cipher

Uses a keystream generator to encrypt data 1 bit at a time

This is generally done with an XOR and is symmetric

Common algorithms are
- [[Diffe-Hellman]]
- [[RSA]]
- [[ECC]]

## Block cipher

Breaks the input into many fixed-length blocks and encrypts each blocks

# References
