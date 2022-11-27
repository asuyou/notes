# access control models
---
Topics: #security 
Created: 2022-07-14 17:07:53

---

You should implicitly deny access to data and apply ideas of least privilege.

You should make it so that it requires multiple people to do sensitive tasks

## DAC

**Discretionary access control**

Policy is determined by the owner and is very common. The issue is that everything must have an owner and permissions set up properly

## Mandatory

Where the computer system chooses who gets permissions based of data labels with trust levels and is implemented on FreeBSD and SE-Linux but is generally used on high-security complex systems

It's always on a need-to-know basis and is implemented via a few methods

### Rule-based

Access based on comparing the subject label and the object label

### Lattice based

Uses complex math to create sets of subjects and object to figure out how they interact

## Role-Based

A model that is controlled by the system but uses a set of permissions rather than just 1

We can move to people into the roles rather than adding individuals

## Attribute-based

Dynamic and context-aware using `if` statements

# References
