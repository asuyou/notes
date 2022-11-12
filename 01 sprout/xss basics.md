# xss basics
---
Topics: [[web]] [[security]] 
Status: #inboxnote
Created: 2022-06-19 18:48:57

---

**Cross Site Scripting**

This is when an attacker embeds a malicious script onto a trusted website

```ad-example
If an attacker made it so a script set by them is run by the victim every time they visit the website https://google.com
```

The victim here is the user

To prevent we need proper [[sanitization]] of all inputs

## Persistent

Attempts to get data provided by the user stored on the web server by the victim

## Reflected

Attempts to have a non-persistent effect on the victim

## DOM based

Attempts to exploit the browser itself

```ad-note
When a script exploits a specific browser like firefox
```

# References
