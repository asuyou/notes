# ipv6 phone networks
---
Topics: [[ipv6]] [[mobile network]]
Status: #inboxnote
Created: 2022-06-24 15:22:52

---

This is based on [[3gpp]] architecture

```txt
                                +-----+    +-----+
                                | AAA |    | PCRF|
                                +-----+    +-----+
              Home Network         \          /
                                    \        /                       /-
                                     \      /                       / I
  MN     BS                           \    /                       /  n
   |     /\    +-----+ /-----------\ +-----+ /-----------\ +----+ /   t
 +-+    /_ \---| ANG |/ Operator's  \| MNG |/ Operator's  \| BR |/    e
 | |---/    \  +-----+\ IP Network  /+-----+\ IP Network  /+----+\    r
 +-+                   \-----------/    /    \-----------/        \   n
                       ----------------/------                     \  e
                     Visited Network  /                             \ t
                                     /                               \-
         +-----+ /------------------\
         | ANG |/ Visited Operator's \
         +-----+\     IP Network     /
                 \------------------/
```

- [[mn]]: mobile note
- [[apn]]: access point name (similar to a SSID)
- [[bs]]: base station
- [[ang]]: access network gateway
- [[mng]]: mobile node gateway
- [[br]]: border router
- [[aaa]]: Authentication, Authorization, and Accounting
- [[PCRF]]: Policy and Charging Rule Function

# References
- https://datatracker.ietf.org/doc/html/rfc6342
