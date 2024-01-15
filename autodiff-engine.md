# Autodiff Engine

> Submitted by Group Labs

Write a simple auto differentiation engine entirely in Rust. The following is some code to help you get started.

<https://github.com/GroupLabs/autodiff>

This already builds a computational graph, and allows backward passes for scalar addition, subtraction, division, and multiplication.

Here is the task (in order of difficulty):

- Improve the graph representation; it is difficult to read the current c_graph
- Implementation for non-scalars (perhaps with ndarray)
  - Vectors
  - Matrices
  - Tensors
- Optimizations to make the code simpler, or to improve theoretical performance
- BONUS: write new operations (`EXP2`, `EXP`, `CAST`, `NEG`, etc.).

Suggested resources:

- [Wikipedia - Automatic Differentiation](https://en.wikipedia.org/wiki/Automatic_differentiation)
- [Karpathy's Micrograd Lecture](https://www.youtube.com/watch?v=VMj-3S1tku0&list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ&index=1)
- [Micrograd Repository](https://github.com/karpathy/micrograd)
- [Tinygrad Repository](https://github.com/tinygrad/tinygrad) - This one is a little more complex, but may be interesting
