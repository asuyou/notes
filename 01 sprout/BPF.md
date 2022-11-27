# BPF
---
Topics: #packet-capture #response
Created: 2022-10-21 14:44:53

---

**Berkeley Packet Filter**

A way of filtering packets using 1 or more primitives followed by qualifiers

We can use `tcpdump` to apply a filter on a data e.g. this on a [[pcap]] file

```
tcpdump -r <filename> [BPF filters]
```

A fun thing I found: For some reason, `tcpdump` gives different outputs even when running on the exact same data and no filters

This is when we output to a file the packets, e.g. `(some command) > a`

# References
- https://biot.com/capstats/bpf.html
- https://blog.cloudflare.com/bpf-the-forgotten-bytecode/
- https://andreaskaris.github.io/blog/networking/bpf-and-tcpdump/