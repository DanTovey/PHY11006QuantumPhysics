(topic4)=
# Introduction to quantum theory

We now take a brief look at the modern approach to describing quantum phenomena, which is know as "quantum theory" or "quantum mechanics". This is much more abstract than what we have discussed so far, and indeed the physical meaning of many of the mathematical concepts introduced by quantum mechanics are still under debate. The mathematics can give rise to some extremely counter-intuitive and bizarre consequences. Nevertheless, the theory is completely consistent with every single experimental test that has been carried out in the past century, in some cases to more than ten decimal places of precision. So although we still do not *understand* quantum mechanics, we can be pretty certain that it *works*.


## The wavefunction

We start by considering the electron trapped in the infinite one-dimensional potential well considered in Topic 3. We have established that it can be described by a de Br&ouml;glie wave, however we have ignored one important fact -- what is physically oscillating in the wave? In quantum mechanics (QM) we do not answer this question directly, but rather we say that the wave is related in a simple mathematical way to another quantity which does have a physical interpretation. 

```{figure} psi.png
:name: fig:psi
:align: center
The wavefunction (a) and probability density (b) for the one-dimensional infinite potential well.
```  

Lets describe mathematically the de Br&ouml;glie wave at a fixed time $t$ with a *wavefunction* $\psi(x)$. If the potential well extends from $x=0$ to $x=L$, then for a standing wave anchored with a node at $x=0$, $\psi(x) = A \sin kx$ inside the well, where $A$ is the amplitude and $k$ is the wavenumber. By requiring that we fit an integer number of half-wavelengths inside the box, so that there is also a node at $x=L$ (see {numref}`fig:psi`(a)), we require that $kL=n\pi$ and hence $k=n\pi/L$. We still have not said what $\psi(x)$ represents physically yet, however this mathematical function is exactly the one which we would use to describe the displacement of a standing wave on a one-dimensional string. 

The physical interpretation of the wavefunction arises from the "Born rule", which states that the modulus squared of $\psi(x)$, namely $P(x)=|\psi(x)|^2 = \psi^*(x)\psi(x)$, is equal to the probability density of finding the electron between $x$ and $x+{\rm d}x$ at the fixed time $t$ (see {numref}`fig:psi`(b)). We use the modulus because, in general, $\psi(x)$ can be complex. Given that the electron must be found *somewhere* we obtain the "normalisation condition" 
```{math}
:label: eqn4.1
\int^{+\infty}_{-\infty} P(x) {\rm d}x = \int^{+\infty}_{-\infty} |\psi(x)|^2 {\rm d}x = 1.
```  
The fact that we do not expect to find the electron outside the potential well implies that $P(x)=0$ and hence $\psi(x)=0$ everywhere outside the well. This allows us to reduce the normalisation condition in the case of this potential well to 
```{math}
:label: eqn4.2
\int^{L}_{0} |\psi(x)|^2 {\rm d}x = 1.
```  
This condition allows us to determine the amplitude (or *normalisation*) $A$ of the wavefunction as follows: 
```{math}
:label: eqn4.3
\begin{aligned}
\int^{L}_{0} |\psi(x)|^2 {\rm d}x = 1 &= A^2 \int^{L}_{0}  \sin^2 \left(\frac{n\pi x}{L}\right) {\rm d}x \cr
&= \frac{A^2}{2} \int^{L}_{0}  1-\cos \left(\frac{2n\pi x}{L}\right) {\rm d}x \cr
&= \frac{A^2}{2} \left[ x-\frac{L}{2n\pi}\sin \left(\frac{2n\pi x}{L}\right) \right]_0^L \cr
&= \frac{A^2 L}{2}.\nonumber
\end{aligned}
``` 
Consequently, we find that $A=\sqrt{2/L}$ and so finally 
```{math}
:label: eqn4.4
\psi(x) = \sqrt{\frac{2}{L}}\sin\left(\frac{n\pi x}{L}\right).
``` 

## The Schr&ouml;dinger equation

So far, we have considered only a simple one-dimensional potential well of infinite depth. In general, we would like to be able to calculate the wavefunction for a particle moving in any three-dimensional potential $V(\vec{x})$, irrespective of whether it is trapped in the well or not. In QM, the wavefunction is the solution to a second-order linear differential equation called the Schr&ouml;dinger equation. This equation is obtained by using *Hamiltonian mechanics* (a framework for calculating the motion of classical particles, based on conservation of energy) and then replacing kinematic quantities such as energy, momentum and position with equivalent mathematical objects called *operators*. This derivation is beyond the scope of the first year course, but will be discuss in the second year QM course.

For a one-dimensional system at fixed time $t$ the full three-dimensional, time-dependent, Schr&ouml;dinger equation reduces to the one-dimensional time-independent Schr&ouml;dinger equation (TISE): 
```{math}
:label: eqn4.5
-\frac{\hbar^2}{2m}\frac{{\rm d}^2\psi(x)}{{\rm d}x^2} + V(x)\psi(x) = E\psi(x),
```  
where the first term corresponds to the kinetic energy of the particle, the second term corresponds to its potential energy, the third term corresponds to its total energy, and $m$ is its mass.

For a one-dimensional infinite potential well, as we considered previously, we can set the potential $V(x)=0$ in the range $0<x<L$, inside the well, and $V(x)=+\infty$ elsewhere. Inside the well the TISE therefore reduces to 
```{math}
:label: eqn4.6
-\frac{\hbar^2}{2m}\frac{{\rm d}^2\psi(x)}{{\rm d}x^2} = E\psi(x),
```  
which is just the one-dimensional wave-equation, with general solution 
```{math}
:label: eqn4.7
\psi(x) = A\sin kx + B\cos kx,
```  
where $k = \sqrt{2mE}/\hbar$, consistent with what we found for de Br&ouml;glie waves previously. Outside the well, when $x\leq0$ or $x\geq L$, the only way to get a finite value of the energy $E$, given that $V(x)=+\infty$, is to set $\psi(x)=0$.

We now need to consider the boundary conditions that apply to $\psi(x)$. In the simple case of the one-dimensional infinite potential well there is only one requirement that applies -- that the wavefunction be continuous (in a mathematical sense) everywhere. Since $\psi(x)=0$ outside the well, this means that $\psi(x)=0$ at the boundaries at $x=0$ and $x=L$. This implies that there must be nodes in the wavefunction at the walls of the well, and so $B=0$ and $k= n\pi/L$, which is again consistent with what we found for de Br&ouml;glie waves previously. We now have two expressions for $k$, which must be equal. In other words $k = \sqrt{2mE}/\hbar = n\pi/L$ and so finally, after rearranging, we find 
```{math}
:label: eqn4.8
E = \frac{n^2\pi^2\hbar^2}{2mL^2},
```  
which is again consistent with what we found for de Br&ouml;glie waves previously.

We will examine the Schr&ouml;dinger equation in much greater depth in the second year course -- in fact it is the main subject of the full 30 lecture course. The Schr&ouml;dinger equation leads us to predict some very strange physics, including phenomena such as quantum tunneling, in which particles can escape from potential wells in which, according to classical physics, they should be trapped. These counter-intuitive predictions have all been observed in nature however, and so we have no reason to think that these predictions are wrong. 
