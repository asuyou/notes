# port knocking
---
Topics: [[ports]] [[networking]]
Status: #inboxnote
Created: 2022-11-02 19:09:27

---

One way to prevent brute force attacks is port knocking.

A server will listen for knocks on specific ports in a specific order; if done right will open up another port the client can connect to.

We can use the `knock` command to achieve this

Syntax

`knock <ip address> [port 1] [port 2] ...`

# References
