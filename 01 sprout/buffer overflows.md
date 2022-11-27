# buffer overflows
---
Topics: #security #buffer-overflows #binary-exploitation
Created: 2022-06-17 18:08:45

---

At the core, this is when a process stores data outside the data range that it should be allowed.

This is used by attackers commonly to change data they shouldn't have access to like RIP pointers and return addresses

Over 85% of breaches were caused b overflows

This can generally be prevented with [[canary tokens]] for basic examples

Injecting [[shellcode]] is into these buffers can also generally be prevented with [[nx]] bits

# References
