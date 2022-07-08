# SQL injection basics
---
Topics: [[sql]] [[web]] [[security]]
Status: #inboxnote
Created: 2022-06-19 19:06:40

---

It is how some apps communicate with databases

An injection is when a user inserts a SQL query that is then run

This is generally done by input fields

```ad-example

A normal query might look like after a user inputs the name `foo`

`SELECT * FROM Users WHERE name="foo"`

If the user instead puts their name as `{backtick} OR 1=1;`
This is then

`SELECT * FROM Users WHERE name="{backtick} OR 1=1;"`

The database will always return true as 1 is always 1
```

To prevent we need to have proper [[sanitization]] by checking if there is an escape character or making sure the entire query cannot be escaped

If we also introduce the concept of least privilege it becomes even harder

# References
