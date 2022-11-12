# zone transfers
---
Topics: [[networking]] [[DNS]] [[security]]
Status: #inboxnote
Created: 2022-11-02 19:15:36

---

This is an attack on DNS. It comes into place during recon stage of a test. It allows us to understand the topology of an organizations DNS network to identify domains that are vulnerable.

It allows us to get all information on a specific DNS servers zone.

> This should be protected but clearly it isn't always

```ad-example
We can test this with a command like the following
`dig @<DNS server IP> axfr <domain name>`
```

# References
