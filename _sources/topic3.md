(topic3)=
# De Br&ouml;glie Waves

Having examined the quantum nature of light, we now turn our attention to the nature of matter. We have seen that light, which classically is viewed as an electromagnetic wave, can also be viewed as being composed of discrete packets or particles of energy. On the other hand, we classically view matter as being composed of particles (such as the electron or atomic nucleus) -- could these conversely be viewed also as waves?

## Wave-particle duality

The equations of special relativity (beyond the scope of this course) require that the energy ($E$), momentum ($p$) and rest mass ($m_0$) of a particle are related by 
```{math}
:label: eqn3.1
E^2 = p^2c^2 +m_0c^4,
``` 
where $c$ is the speed of light. If the particle is massless, as is the case for a photon, then $m_0=0$ and so $p=E/c$. But we have already seen that $E=hf=hc/\lambda$ and so this implies that 
```{math}
:label: eqn3.2
p=\frac{h}{\lambda}.
```  
This holds for photons -- could it hold also for matter particles such as electrons? De Br&ouml;glie proposed in 1924 that it should (the de Br&ouml;glie hypothesis).

If the de Br&ouml;glie hypothesis is correct then a stream of particles should behave as a wave in certain circumstances, with a de Br&ouml;glie wavelength $\lambda$. We can calculate $\lambda$ if we know the momentum or kinetic energy of the particles. For instance, we can take the non-relativistic expression linking kinetic energy $E_K$ with momentum, $E_K = p^2/2m$, and write it in terms of the wavelength of the particle: 
```{math}
:label: eqn:hbk2m
E_K = \frac{h^2}{2m\lambda^2} = \frac{\hbar^2k^2}{2m},
\label{eqn:hbk2m}
``` 
where we have introduced the *wavenumber* $k= 2\pi/\lambda$ in the last step as we shall need it below. Rearranging this expression we find that $\lambda = h/\sqrt{2 m E_K}$. If we evaluate $\lambda$ for different objects and particles we find that it is negligibly small for macroscopic objects (tennis balls, cars, the earth etc.) but can be as large as $10^{-10}$ m for electrons accelerated to high energy. This distance is similar to the separation between atoms in crystals, and therefore we expect to see wavelike behaviour such as diffraction and interference for electrons passing through crystal lattices. This is in fact observed and forms the basis for the Transmission Electron Microscope (TEM) used throughout physics, chemistry and biology today.

## Standing de Br&ouml;glie Waves

```{figure} 1dbox.png
:name: fig:1dbox
:align: center
de Br&ouml;glie waves of an electron trapped in a one-dimensional infinite potential well.
``` 

If matter can be regarded as being composed of waves then it should obey the laws of physics that apply to waves. If a matter particle such as an electron is trapped in a one-dimensional potential well of infinite depth, then its de Br&ouml;glie wave cannot escape outside of the well -- it is confined to the well. This situation is rather like a one-dimensional string anchored between two fixed points -- in that case the string does not extend beyond either of the anchor points. When one oscillates such a string, a standing wave is formed, with nodes at each of the anchor points and possibly additional nodes along the string depending on the order of the mode that has been excited. The same should be true for our trapped electron -- its de Br&ouml;glie wave should become a standing wave with nodes at the walls of the potential well and possibly additional nodes inside the well. We can satisfy this requirement if we can fit an integer number of half-wavelengths inside the well (see {numref}`fig:1dbox`). The wavelengths of the standing waves are the same for the electron as for the string -- they are $\lambda = 2L/n$, where $L$ is the width of the well (or separation of the string anchors) and $n=1, 2, \dots$ is the number of anti-nodes in the well (or on the string). Equivalently, the wavenumber is given by $k=n\pi / L$. We can now calculate the kinetic energy of the electron using Eqn. {eq}`eqn:hbk2m` 
```{math}
:label: eqn3.4
E_K = \frac{\hbar^2k^2}{2m} = \frac{n^2\pi^2 \hbar^2}{2mL^2}.
```  
This expression depends on an integer ($n$) and hence the kinetic energy of the electron is no longer continous but rather discrete - i.e. the energy is *quantised*. Quantisation of energy levels is a consequence of the wave nature of the particle considered. Quantisation effects become important when the separation between the energy levels of a particle or object becomes much larger than its thermal energy. This is almost never the case in the world around us, so macroscopic objects do not display obvious energy quantisation behaviour, however it can occur in systems that are very cold (low thermal energy) or very small (small $L$ and hence relatively large energy level separation).

Given our new understanding of the wave nature of matter, we are now able to understand the origin of Bohr's fourth postulate -- that the magnitude of the angular momentum of electrons orbiting atoms should be quantised. We can think of a circular orbit as being like a periodic one-dimensional potential well where the displacement (and gradient) of the wave at one boundary is equal to that at the other boundary. This, in fact, requires that we can fit an integer number of full (not half) wavelengths along the orbit, and so $2\pi r = n \lambda$ and hence $\lambda = 2\pi r/ n$. The de Br&ouml;glie hypothesis combined with the expression for the magnitude of the angular momentum  gives $L = m_e vr = p r = hr/\lambda$ and so finally $L= nhr/2\pi r= n \hbar$, as required.


