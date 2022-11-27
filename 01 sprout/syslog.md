# syslog
---
Topics: #protocol
Created: 2022-07-15 21:13:05

---

This is a protocol allowing different applications to transmit logs to central server using a client-server model. However, as it uses UDP, there can be issues in congested networks and has no security 

This can be used to data to the [[SIEM]]

They contain a PRI code (priority), a header and a message portion

In newer versions, it uses `1468` on TCP for consistent delivery, can use TSL to encrypt, can use MD-5 or SHA-1 for auth and integrity.
They can also have features like
- Message filtering
- Automated log analysis
- Event response
- Alternate message formats

# References
