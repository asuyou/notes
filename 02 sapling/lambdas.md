# lambdas
---
Topics: [[programming]] [[reverse engineering]]
Status: #inboxnote
Created: 2022-06-14 09:53:51

---

These are also known as [[anonymous functions]]

It's really useful to create lambda functions for common things to make them shorter
e.g.

```python
p64 = lambda x: struct.pack("Q", x)
pd = lambda x: b"A"*x
```

These are just small functions that are meant to be short and small.

# References
- https://docs.python.org/3/library/struct.html#format-characters
- https://realpython.com/python-lambda/
