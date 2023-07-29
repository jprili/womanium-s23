# Circuits and Algorithms

Now that we know what qubits are ([see previous article](https://github.com/jprili/womanium-s23/blob/main/src/intro.md)),
let us now move on utilising qubits for computing.

## Reversible Computing in QC systems
Reversible computing is, to put simply,
a method of computing that is able to get the input state from the output state.
Take the classical AND gate. The truth table shows:

| in0 | in1 | out |
|-----|-----|-----|
|  0  |  0  |  0  |
|  1  |  0  |  0  |
|  0  |  1  |  0  |
|  1  |  1  |  1  |

This is an example of **non-reversible** computing.
If given of output of 0, 
there is no way to determine what values `in0` and `in1` were before applying the gate,
unless it was measured before, which is what a reversible AND gate would be.

| in0 | in1 | in2 | out0 | out1 | out2 |
|-----|-----|-----|------|------|------|
|  0  |  0  |  0  |  0   |  0   |  0   |
|  1  |  0  |  0  |  1   |  0   |  0   |
|  0  |  1  |  0  |  0   |  1   |  0   |
|  1  |  1  |  0  |  1   |  1   |  1   |

In quantum computing, operations on qubits **must** be reversible.
It stems from quantum mechanics' unitarity (meaning, and what enables qubits to be entangled.
