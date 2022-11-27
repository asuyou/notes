# ECC
---
Topics: #encryption
Created: 2022-07-17 18:16:29

---

**Elliptic Curve Cryptography**

[[encryption|Encryption]] based on algebraic structure of elliptical curves over finite fields.

It is significantly more efficient than other methods and very fast while still having ample security

ECC with `256` bit key is as secure as [[RSA]] with a `2048` bit key

Used on devices with lower computational power

## Math

These curves are in the form of $y^2 = x^3+ax+c$ and this leads to symettry around the $x$-axis which is used later in the equation.

```ad-example
The `secp256k1` use the equation $y^2=x^3+7$ and is used in bitcoin
```

There is an additive property in these curves where if we choose 2 points on the curve and draw a line between them, then find another point on the curve that the line intersects and mirror the point across the axis, we get what we would if we just added the points

```ad-note
It looks something like this

![Curve](https://hackernoon.com/hn-images/1*dErGh_rL2ExM6AX-Rtyb7w.png)

$$P+Q=R$$
```

This is the start. For more details read the article

# References
- https://hackernoon.com/what-is-the-math-behind-elliptic-curve-cryptography-f61b25253da3