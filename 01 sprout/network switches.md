# network switches
---
Topics: [[networking]] [[spoofing]]
Status: #inboxnote
Created: 2022-07-07 19:36:34

---

Combined versions of hubs and bridges

Switches can be configured to support [[VLAN]]s

## MAC flooding

Attempt to overwhelm the memory set aside to store MAC addresses for each port

If it is flooded it can fail-open and act like a hub (sending data to all devices)

## MAC spoofing

When an attacker masks own MAC address

```ad-example
A WAP might be setup to only allow certain MAC addresses. If a new device spoofs to have one of these addresses, it can then use the network
```

This is generally combined with [[ARP  spoofing]]

To prevent this you need to limit the static MAC addresses accepted and limit the duration of time for ARP entry on host and conduct ARP inspection

# References
