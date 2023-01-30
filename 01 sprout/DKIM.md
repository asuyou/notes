# DKIM
---
Topics: #email #security #dns
Created: 2022-12-22 01:01:37

---

**Domain Keys Identified Mail**

Authentication method attacked to emails that aims to prevent using a false sender email

Does this using a signature linked to a domain which is attached on outgoing messages

This is based on [[cryptography]], specifically public key where a mail server generates its own keys and hosts a public DNS record with public key to verify the signature

# References
- https://en.wikipedia.org/wiki/DomainKeys_Identified_Mail
- https://www.cloudflare.com/learning/dns/dns-records/dns-dkim-record/
