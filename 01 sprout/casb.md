# casb
---
Topics: [[cloud]] [[security]]
Status: #inboxnote
Created: 2022-07-08 23:48:22

---

**Cloud Access Security Broker**

This is an enterprise management software designed to mediate access to cloud by users

This is basically a middle step between users and the cloud but they do provide things like
- [[sso]] and enforce access controls
- malware and rouge device detection
- monitor user activity
- mitigate data ex filtration

They allow you to see how users interact with cloud

They can be setup in a few different ways

## Forward proxy

A security appliance or host on the client network that forwards traffic to the cloud network

## Reverse proxy

An appliance positioned on the cloud network and directs traffic to the cloud services if data complies with the policy

## API

**Application Programming Interface**

A method that uses the broker's connection between the cloud service and consumer

It generally does not have great policy support as in-depth policies may not be implemented

# References
