# secure development concepts
---
Topics: #security #software #development
Created: 2022-06-17 17:38:27

---

## Least Privilege

Users and processes should be run using the least amount of access necessary to perform the function given

## Defense in Depth

This is just layering multiple controls to increase the security of a system rather than relying on a single control

## Sanitize user input

User input needs to validated and corrected to ensure it cannot damage the application in any way

## Minimizing attack surface

```ad-attention
If there is no, there can be no bugs
- Sun Tzu (probably)
```

If we reduces the amount of code used by removing unneeded functionality and require [[authentication]] before allowing additional plugins

## Create Secure Defaults

Default installations should be secure by default

## Code Signing

Code signing allows us to ensure that programs has not been changed in any way before a user runs this

This is similar to using things like MD5 sums and hashes

## Secure Failing

Applications will fail

So when they fail they need proper exception handling

## Rely on trusted SDKs

These must come from trusted sources to ensure no malicious code is inserted into the end user app by accident

# References
