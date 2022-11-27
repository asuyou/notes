# ports
---
Topics: #networking
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

We want to minimize the number of ports open to just the ones necessary

We can shutdown the service opening the ports with
Window : either GUI or `net stop <service>`
Linux: `sudo stop <service>`

We can block with the firewall

## Ports for SEC+

These are the ports and protocols that need to be remembered

| Port       | Protocol                            | TCP / UDP |
| ---------- | ----------------------------------- | --------- |
| 21         | FTP                                 | TCP       |
| 22         | SSH / SCP /SFTP                     | Both      |
| 23         | Telnet                              | Both      |
| 25         | SMTP                                | TCP       |
| 53         | DNS                                 | Both      |
| 69         | TFTP (Trivial FTP)                  | UDP       |
| 80         | HTTP                                | TCP       |
| 88         | [[kerberos]] (windows network auth) | Both      |
| 110        | POP3                                | TCP       |
| 119        | [[NNTP]]                            | TCP       |
| 135        | RPC (To locate DCOM)                | Both      |
| 137 -> 129 | NetBIOS                             | Both      |
| 143        | IMAP                                | TCP       |
| 161        | [[SNMP]]                            | UDP       |
| 162        | SNMPTRAP                            | Both      |
| 389        | [[LDAP]]                            | Both      |
| 443        | HTTPS                               | TCP       |
| 445        | SMB                                 | TCP       |
| 465/587    | SMTP (with TLS)                     | TCP       |
| 514        | [[syslog]]                          | UDP       |
| 636        | LDAP (TLS)                          | Both      |
| 869        | [[iSCSI]]                           | TCP       |
| 989/900    | FTPS                                | TCP       |
| 993        | IMAP4 (TLS)                         | TCP       |
| 995        | POP3 (TLS)                          | TCP       |
| 1433       | MS-SQL-Server                       | TCP       |
| 1645/1646  | RADIUS                              | UDP       |
| 1701       | L2TP (VPN)                          | UDP       |
| 1723       | PPTP                                | Both      |
| 1812/1813  | [[radius]] (defaults)               | UDP       |
| 3225       | FCIP                                | Both      |
| 3260       | iSCSI Target                        | TCP       |
| 3389       | [[RDP]]                             | Both      |
| 3868       | Diameter                            | TCP       |
| 6514       | Syslog (TLS)                        | TCP       |

# References
