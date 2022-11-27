# NOP slide
---
Topics: #security #binary-exploitation
Created: 2022-06-17 18:23:54

---

If a buffer is filled with NOPs until we slide down and find the [[shellcode]]

This can make [[ASLR]] obsolete as even it jump to a random area in memory, it will still be in the same general area so if we fill up the area with NOPs and then some shellcode, we will always slide down to it. 

# References
