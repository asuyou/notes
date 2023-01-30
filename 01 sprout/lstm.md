# lstm
---
Topics: #ai #math #lstm #nn
Created: 2023-01-26 13:22:42

---

These are a very specific type of [[RNN]] that are used for long-term learning. Using these is very useful for things like predicting time-series data.

Similar to [[RNN]]s, they also have a chain structure but have multiple [[nn]] layers in-between

![LSTM chain](https://colah.github.io/posts/2015-08-Understanding-LSTMs/img/LSTM3-chain.png)

Instead of a single $\tanh$ we have 3 $\sigma$ layers and a $\tanh$ layers.

This is all within a single LSTM cell.

The cell state is generally controlled by a few different aspects called gates.

## Forget gate

This is controlled by a sigmoid gate. It considers $h_{t-1}$ and $x_t$ and produces an output for  each number in the cell.

## Keep gate

Comprised of the middle section where we first have $\sigma$ as an "input gate layer" and then a $\tanh$ layer to create a vector of new values.

We then update the old cell state $C_{t-1}$ into the state of $C_t$

# References
- https://colah.github.io/posts/2015-08-Understanding-LSTMs/
