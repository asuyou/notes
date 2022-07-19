# VPN protocols
---
Topics: [[protocol]] [[security]]
Status: #inboxnote
Created: 2022-07-19 23:46:53

---

> These are pretty old huh

### PPTP

Protocol that encapsulates PPP packets and sends out encrypted traffic

## L2TP

Layer 2 tunneling protocol but is not secure

Used on port `1701` from [[ports]]

## IPSec

TCP protcol that encrypts and authenticates and sends packets using [[IKE]] using either main mode, aggressive mode or quick mode.

It uses security association to verify identities, authentication headers to provide integrity and authentication and encapsulating security payload provides some confidentiality by encrypting and encapsulating them.

We have transport mode where the payload is encrypted but the headers are not. Tunnel mode encrypted the entire packet including header.

# References
