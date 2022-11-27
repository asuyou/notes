# network zones
---
Topics: #networking
Created: 2022-07-07 20:15:29

---

## LAN

Local area network

## WAN

Wide area network

## DMz

De-Militarized Zone

Focused on providing controlled access to publicly available server that are hosted within network

This should be secure and tightly locked down and is isolated from the rest of the network by firewalls that generally accepts connections from the internet over set ports

```ad-example
If you self-host an email server, it would be placed here
```

### Extranet

Special type of DMZ that is created for partner organizations to access over a wide network

### Bastion Hosts

Hosts or servers in the DMZ which are not configured with any services that run on the local network

### Jumpbox

This is a server that we can configure and that allows us to access other hosts in the DMZ

# References
