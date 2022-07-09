# ports
---
Topics: [[networking]]
Status: #inboxnote
Created: 2022-07-09 20:18:50

---

A communication endpoint that exists on a computer or server

```ad-example
Port 80 and 443 will be open on a web server
```

There are inbound ports for listening to connections

Out-band ports are opened when a client tries to connect to another device. This is generally a high point

```ad-example
A server has port `22` open for ssh and a client opens port `54433` to communicate
Data is then sent back from the server to the client to that high port
```

Ports range between `0` and `65_535`

This is split into 3 groups
1. Well known ports `0 -> 1023` as they are assigned by IANA
2. Registered ports `1024 -> 49_151` that are assigned to proprietary protocols by IANA
3. Dynamic/Private ports `49_152+` these can be used by any application

## Ports for SEC+

These are the ports and protocols that need to be remembered

| Port       | Protocol                        | TCP / UDP |
| ---------- | ------------------------------- | --------- |
| 21         | FTP                             | TCP       |
| 22         | SSH / SCP /SFTP                 | Both      |
| 23         | Telnet                          | Both      |
| 25         | SMTP                            | TCP       |
| 53         | DNS                             | Both      |
| 69         | TFTP (Trivial FTP)              | UDP       |
| 80         | HTTP                            | TCP       |
| 88         | Kerberos (windows network auth) | Both      |
| 110        | POP3                            | TCP       |
| 119        | [[NNTP]]                        | TCP       |
| 135        | RPC (To locate DCOM)            | Both      |
| 137 -> 129 | NetBIOS                         | Both      |
| 143        | IMAP                            | TCP       |
| 161        | [[SNMP]]                        | UDP       |
| 162        | SNMPTRAP                        | Both      |
| 389        | [[LDAP]]                        | Both          |


# References
