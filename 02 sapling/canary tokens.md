# canary tokens
---
Topics: #binary-exploitation #security
Created: 2022-05-29 10:12:13

---

They are a value placed onto the stack at the start. It changes every time the program is run and before a return, it is checked. If it is different due to being overwritten, then the program exits immediately.

This makes it hard to overwrite a return address as if we change it to a random arbitrary value, we get stack smashing 

They generally end in `00` as in [[little endian]] format they null-terminate strings but it makes them easier to spot

These are not 100% secure but a little bit of security

Overwriting one of these with the wrong one will lead to errors like [[stack smashing]]

# References
- https://corruptedprotocol.medium.com/killer-queen-ctf-tweety-birb-canary-bypass-with-format-string-vulnerability-2f1f3b516fe2
- https://ctf101.org
- https://ir0nstone.gitbook.io/notes/types/stack/canaries#:~:text=On%20Linux,%20stack%20canaries%20end,them%20much%20easier%20to%20spot.
