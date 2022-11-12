# Canary Bypass With FMTS
---
Topics: [[canary tokens]] [[reverse engineering]] [[ret2win]] [[format string]] [[security]]
Status: #inboxnote
Created: 2022-05-29 10:13:12

---

If we look at [[canary tokens]] we see that they end in `00`

If we can get the program to print a [[format string]] then we can leak values from the [[stack]] including the canary token

We can do this with input like the one below which we can then find the position of the value that always ends in `00`.

```python
print(b"%p." * 10)
# %p.%p.%p.%p.%p.%p.%p.%p.%p.%p.
```

```ad-note
Rerun this multiple times to make sure the position is the right one as there might be other values that end in `00`
```

If we see that it is always the 4th value, from then on we can just use `%4$p` instead

# References
- https://corruptedprotocol.medium.com/killer-queen-ctf-tweety-birb-canary-bypass-with-format-string-vulnerability-2f1f3b516fe2
