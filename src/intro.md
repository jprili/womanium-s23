# Qubits and Quantum Physics
Before talking about Quantum Computing,
it would be ideal to discuss concepts in computing and quantum physics first.

## Classical Computers  
A computer generally refers to a machine that does arithmetic and logical operations.
To satisfy this definition, a computer would first need to have some way to represent the logic state.
This "logic state" will be called a **bit**, a shorthand for "binary digit", which is a set containing two values: 0 or 1, `true` or `false`.
Other representations are also used.
It will be the fundamental logic element that a classical computer will build upon for its operations.
Hardware-wise, this is achieved via transistors and/or magnetic memory spin, 
where the bit representation is analogous to the prescence of current running through them.

## Quantum Physics
As computers improve over time, the scale at which the basic logic operation takes place in decreases.
Processors get smaller and smaller, some computers 
[as tiny as 1 mm x 1 mm](https://www.theverge.com/circuitbreaker/2018/3/19/17140116/ibm-worlds-smallest-computer-grain-of-salt-solar-powered) 
even.
A consequence of this is that at for the components of the hardware this scale, 
quantum physics starts to take over; 
there will be phenomena that can not be easily explained by classical mechanics alone (e.g. shot noise, light polarisation).

Particles in the quantum regime behave differently compared to their classical counterparts, 
as demonstrated in the 
[*double-slit experiment*](https://www.olympus-lifescience.com/en/microscope-resource/primer/java/doubleslitwavefronts/).
It shows that very small particles such as photons and electrons,
behave in a way where the particle can be in **more than one state at a time**,
in the case of the experiment, the position state is the one in superposition.
It also showed that these quantum states can be represented in the form of a wave (for continuous states).

This wave state is called a *wavefunction*. It is usually written as $\ket{\Psi}$.
The wavefunction contains all the information needed to describe the **full** state of a quantum system. 
A quantum particle, for example, can contain both the momentum and the space information in the wavefunction.

Measuring the state collapses the wavefunction, 
as in the other properties of the wavefunction will disappear and "reduce" to the property measured.
This is due to the measurement process involving a particle interacting with the one measured.
For example, in the double-slit experiment, the particles that pass through the slit interacts with the surface which collapses the wavefunction that it had prior.

## Qubits  
A Qubit can be thought of as a wavefunction in state $\ket{q}$:  
Let $\ket{0} = \[1 ~ 0\]^{T}$, and $\ket{1} = \[0 ~ 1\]^{T}$;
$$\ket{q} = \alpha \ket{0} + \beta \ket{1}$$
where $|\alpha|^{2} + |\beta|^{2} = 1$ (normalisation),
and $|\alpha| ^ {2}$ and $|\beta| ^ {2}$ are probabilities to find the qubit being in $\ket{0}$, $\ket{1}$ respectively.  
The advantage this gives us over classical bits is that the qubit can store more information, with the difference being more noticeable with increasing bits/qubits.  

From [Microsoft Azure](https://azure.microsoft.com/en-ca/resources/cloud-computing-dictionary/what-is-a-qubit/):

> - The amount of information a qubit system can represent grows exponentially. Information that 500 qubits can easily represent would not be possible with even more than 2^500 classical bits.
> -  It would take a classical computer millions of years to find the prime factors of a 2,048-bit number. Qubits could perform the calculation in just minutes.

Qubits can also be geometrically represented as points on the surface of a sphere.
The axes [represent different states](https://www.sharetechnote.com/html/QC/QuantumComputing_BlochSphere.html), such as:

$$\ket{+} = \frac{1}{\sqrt{2}} \ket{0} + \frac{1}{\sqrt{2}} \ket{1}$$  

$$\ket{-} = \frac{1}{\sqrt{2}} \ket{0} - \frac{1}{\sqrt{2}} \ket{1}$$

Measuring these states would collapse the qubits into $\ket{0}$ or $\ket{1}$, with 0.5 probability for each.

<p align="center" width="100%">
    <img width="50%" src="https://www.sharetechnote.com/html/QC/image/QuantumComputing_BlochSphere_10.png">
</p>

The image above shows the axes and the corresponding states that they represent. 
Image from *ShareTechNote* website.


Operating on qubits requires the use of Quantum logic gates, which will be discussed in the next article.

