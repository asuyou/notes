# PIE and Canary bypass with offsets
---
Topics: [[canary tokens]] [[ret2win]] [[pie]] [[security]]
Status: #inboxnote
Created: 2022-06-13 20:27:26

---

Offsets are always constant and so are the [[pointers]] that we get back from popping data from the [[stack]] are the same every time we run it

We can [[leak values from the stack]] with `%n$lx` or `%n$p` which are roughly equivalent. These are just [[format string]]

If we can leak a value from the stack with a pointer to another function of our program, we can calculate the offset from either the entry point of our binary or libc

From there we can calculate the dynamic address of any other function e.g. a [[ret2win]] function

That's the plan

In action what we can do is supply input and see the offset from that input where a value that would return us to the program is. If we also calculate the offset of our input and where the stack starts printing from, we can find the the total offset and use that. 

# References
- https://www.youtube.com/watch?v=FpKL2cAlJbM
- https://en.wikipedia.org/wiki/Printf_format_string
- https://www.quora.com/In-C-why-do-we-use-p-in-printf-statements-instead-of-lx-Arent-they-exactly-equivalent
