# cloud security issues
---
Topics: #cloud #security
Created: 2022-07-08 23:33:18

---

If a cloud server crashes due to 1 organization then many other ones are also affected and this applies to data security as well

To keep servers from going down, they need to be setup with proper failover and redundancy to keep loads balanced across multiple server

Data that is left behind needs to be looked after. When you deprovision a resource, remnants of that data might be left behind so the next person to provision that space might be able to bring it back and use it

## Insecure API

They should always be over HTTPS with (TLS or SSL) and data received should be sanitized and validated and ensure that error handling is set up.

To prevent DDoS, rate limiting should be implemented

Remember to setup good [[cors]] settings as errors might occur when using things like CDNs

## Improper key management

APIs should be using authentication and authorization like SAML, OAuth and OIDC

```ad-warning
**DO NOT EMBED KEYS IN CODE**. Literally government institutions have done this and have found themselves screwed over by this
```

Also just remember  to delete old keys and generate new ones

## Logging and monitoring

In [[SaaS]] you generally don't have access to log files or monitoring tools

Also copy logs to long-term storage

## Unprotected storage

Buckets or blobs

Access contorl to storage is administered through container policies, IAM authorizations and object ACLs

# References
