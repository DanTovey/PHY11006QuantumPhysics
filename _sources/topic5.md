(topic5)=
# The Heisenberg Uncertainty Principle

One of the more bizarre consequences of quantum mechanics is that there is a fundamental limit on the precision with which certain quantities can be measured simultaneously. This is known as the "Heisenberg Uncertainty Principle" (HUP). It arises from the fact that we describe physical systems with the wavefunction, that is a solution to the Schr&ouml;dinger equation. We can use several thought experiments to justify the HUP in realistic physical systems (see the lecture slides), however it is perhaps easier to get an intuitive feel for it from a more abstract case. 

Consider a particle described by a wavefunction $\psi(x) = A \sin(kx)$. The wavenumber $k=2\pi/\lambda = p/\hbar$ is directly related to the momentum ($p$) of the particle by the de Br&ouml;glie relation $p=h/\lambda$. Since the wavenumber is fixed, so is the momentum $p$. Any measurement of the momentum of this particle will give the same value $p=\hbar k$, and so the uncertainty in the result of this measurement is zero. On the other hand, if we measure the position of the particle, we could find any value between $x=-\infty$ and $x=+\infty$, because the wavefunction is non-zero across the full range of $x$, and the probability of finding the particle at a particular values of $x$ is given by $|\psi(x)|^2$. 

```{figure} wavepacket.png
:name: fig:wavepacket
:align: center
A wavepacket formed from a superpositions of many wavefunctions of different wavenumber and hence frequency.
```  
Now consider what happens when we combine wavefunctions of different wavenumber and hence different wavelength and hence different momentum. The superposition of the wavefunctions forms beat waves of varying amplitude. The more wavefunctions that we add to the superposition, with a broader range of wavenumbers, wavelengths and hence momenta, the more the beats become amplified at one location where they are all in phase. This creates a localised maximum in the combined wavefunction, called a wavepacket (see {numref}`fig:wavepacket`). With some maths (Fourier series or Fourier transforms) one can show that the width of this wavepacket in $x$ is inversely proportional to the range of momenta of the waves that are contributing to the wavepacket. Given that we now have a range of values of momenta, a measurement of the momentum of the particle is no longer fixed but rather could be any one of the values used in the superposition. Hence the result of a measurement of the momentum becomes more uncertain, while the result of a measurement of position (given by the width of the wavepacket in $x$) becomes more precise. Only by combining wavefunctions with an infinite range of momenta (and hence infinite uncertainty in $p$) can we obtain a wavepacket wavefunction that is completely localised in position (giving a perfectly precise measurement of $x$).

Wavefunction solutions to the Schr&ouml;dinger equation, when combined with the Born rule, give rise to exactly the behaviour discussed above. Mathematically, we find that certain pairs of observable quantities can only be measured simultaneously with precisions that are inversely proportional to each other, and so they cannot both be measured simultaneously with total precision. Denoting the uncertainties in measured quantities by $\Delta$ we find that the precisions of simultaneous measurements of position $x$ and momentum $p$ are limited by: 
\begin{equation}
\Delta x \Delta p \geq \frac{\hbar}{2}.
\end{equation} 
Similarly the precisions of simultaneous measurements of energy $E$ and time $t$ are limited by: 
\begin{equation}
\Delta E \Delta t \geq \frac{\hbar}{2}.
\end{equation} 
This has important physical consequences across the whole of physics. For instance, it means that any fundamental particle which has a very short lifetime before it decays (equivalent to $\Delta t$) also must have a very large uncertainty in the value of its mass obtained from a measurement (because $E=mc^2$ and hence $\Delta m = \Delta E / c^2 \geq \hbar / 2 c^2 \Delta t$). 
