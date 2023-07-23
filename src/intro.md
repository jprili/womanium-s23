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
 
