(topic1)=
# The nature of light

We start by looking at the nature of light, as seen by classical physics. Then we look at an experiment whose results cannot be explained in this picture and see how a quantum picture of light can resolve the discrepancy. Finally, we look at another experiment which confirms the quantum picture of electromagnetic radiation.

## Light according to classical physics

Young's double slits experiment (see lecture slides) demonstrates that light propagates as a wave. The light waves from each slit interfere to generate the interference pattern observed on the screen. According to classical physics (Maxwell's equations), the light wave consists of oscillating electric and magnetic fields, polarised at right-angles to each other and propagating in the same direction with the same wavelength and frequency. The light wave moves at the speed of light in the medium through which the wave propagates. This is true for all electromagnetic (EM) waves, e.g. visible light, radiowaves, microwaves, infrared radiation, ultraviolet light, X-rays and gamma rays.

For any kind of classical wave, the intensity ($I$) is defined as the energy flow through unit area per unit time. This is equivalent to the power ($P$) divided by the are ($A$). For EM waves this is given by
```{math}
:label: eqn1.1
I= \frac{c\epsilon_0}{2} E_0^2,
```
where $c$ is the speed of light, $\epsilon_0$ is the permittivity of free space and $E_0$ is the amplitude of the electric field. Most importantly, note that the intensity, and hence power, is independent of the wavelength ($\lambda$) or frequency ($f$) of the wave.

## The photoelectric effect

In a metal, the flow of electric current is due to the flow of charged particles called electrons. The electrons are relatively free to move throughout the metal (an electron "gas" ), so most metals are good conductors of electricity. By shining light on a metal, some of these electrons can be knocked out of the metal to generate an electric current outside of the metal. 
```{figure} pe-expt.png
:name: fig:pe-expt
:align: center
A photoelectric effect experiment.
```
In the "Drude model"  of a metal, there are many free electrons, which behave like an ideal gas of charged particles, with a broad range of velocities (in fact, a Maxwell-Boltzmann distribution) and hence kinetic energies. Because of this large number of free, charged particles, metals are usually very good electrical conductors. Since electrons do not spontaneously leak out of a metal, they must be trapped inside by a potential well -- it takes extra energy for an electron to escape from the metal. The extra energy required for the *most energetic* electrons to escape from the potential well is called the workfunction ($\phi$). This is a property of the metal, but not of the light that shines on it. This energy can be provided by light shining on the metal -- this is the *photoelectric effect*. The ejected electrons are called *photoelectrons*.

In a photoelectric effect experiment (see {numref}`fig:pe-expt`), a metal sample (the cathode) is placed an evacuated glass tube and connected to an electrical circuit. A second electrode (the anode) is also placed in the vacuum tube and connected to the other end of the electrical circuit. The electrical circuit consists of a voltage source (e.g. a battery), a potential divider (variable resistor) to change the voltage provided by the source, and an ammeter to measure the current flowing in the circuit. The voltage source is connected so that the cathode sample can be given a positive (or negative) voltage with respect to the anode. A source of monochromatic (single colour) light is shone onto the cathode, potentially ejecting photoelectrons towards the anode. If these photoelectrons hit the anode then a current flows in the circuit, with a magnitude that is proportional to the number of photoelectrons emitted per unit time.

When no voltage is applied between the cathode and anode and light is shone onto the cathode, the following is observed:
* When the cathode is illuminated with light with a frequency greater than a certain "threshold frequency"  a current is detected, i.e. photoelectrons must be ejected from the metal. 
* Electrons are emitted *instantaneously*, even for lowest intensity of light.
* If the frequency of incident light is below the threshold frequency, no electrons are emitted, no matter how intense the light is.
If light were behaving entirely like a classical EM wave, its power would be proportional to its intensity, but independent of frequency. We would therefore expect that intense light of any frequency to generate photoelectrons, and also that there would be a time delay for emission for light of low intensity, while energy builds up in the sample until it exceeds the workfunction.

When a voltage *is* applied between the cathode and anode and light is shone onto the cathode, the following is observed:
*  When the cathode is illuminated with light with a single frequency greater than the threshold frequency, and the anode-cathode potential difference is such that the cathode is negatively charged and the anode is positively charged, the current is proportional to the intensity of the light (see {numref}`fig:pe-res1`).
*  When the cathode is illuminated with light with a single frequency greater than the threshold frequency, and the anode-cathode potential difference is such that the cathode is positively charged and the anode is negatively charged (so that the flow of negatively charged electrons from cathode to anode is opposed by the applied voltage), the current decreases as the magnitude of the voltage is increased (see {numref}`fig:pe-res1`). The current-flow stops altogether at a particular voltage called the "stopping potential"  ($V_0$).
*  When the wavelength or frequency of the light illuminating the cathode is changed, but the intensity is kept constant, the stopping potential is observed to change as well, and is proportional to the frequency (see {numref}`fig:pe-res2`).
The electrons in the metal do not all have the same kinetic energy (see above), so the stopping potential $V_0$ is the voltage required to stop the *most energetic* electrons from leaving the metal.

```{figure} pe-res1.png
:name: fig:pe-res1
:align: center
Results of the photoelectric effect experiment for light of constant frequency.
```
```{figure} pe-res2.png
:name: fig:pe-res2
:align: center
Results of the photoelectric effect experiment for light of constant intensity.
```

The physics of this system is as follows. The light gives a certain amount of energy $E_p$ to each electron in the cathode. If that energy is great than the workfunction $\phi$, then the most energetic electrons can be ejected from the cathode towards the anode, each with kinetic energy $E_p - \phi$. When the cathode is positively charged and the anode negatively charged, these electrons must do work against the electric field in order to reach the anode and cause a current to flow. The condition that these electrons reach the anode is that their kinetic energy must exceed $eV$, where $V$ is the voltage between the cathode and anode. When $V=V_0$, the current is stopped because the most energetic electrons stop in the applied electric field just before they reach the anode. In this case $E_p - \phi = eV_0$.

Why does the stopping potential depend on the wavelength of the light? Einstein's postulate states that in fact the light is composed of small packets of energy (photons) with zero mass, each of which has an energy
```{math}
:label: eqn1.2
 E_p = hf = \frac{hc}{\lambda},
```
 where $h$ is a new constant (``Planck's constant" ). The intensity of the light is then proportional to the flux of photons -- the number of photons flowing through unit area in unit time. The photons behave like "bullets"  with energy $hf$, which can hit individual electrons. If $f$ is high enough, a single photon can instantaneously remove an electron from the metal. The current of electrons is proportional to the light intensity (if $f$ is above the threshold frequency). The light intensity is equal to the number of photons hitting the cathode surface per second while the current is equal to the number of electrons emitted from the cathode surface per second. 

Putting this all together, we obtain a formula relating the stopping potential $V_0$, the workfunction $\phi$ and the frequency of light $f$: 
```{math}
:label: eqn1.3
eV_0 =hf - \phi.
```
By measuring $V_0$ as a function of $f$ and plotting them together, we obtain a straight line graph with gradient $h/e$ and y-intercept $-\phi/e$ (or equivalently gradient $h$ measured in units of eV s and y-intercept $-\phi$ measured in units of eV). Hence we can simultaneously measure a property of the sample (the workfunction) and a fundamental property of the universe (Planck's constant) using a simple photoelectric experiment!

## The Compton effect

```{figure} compton.png
:name: fig:compton
:align: center
Results of a Compton scattering experiment.
```
Further support for the photon picture of light is provided by observing what happens when light of very high frequency (X-rays) illuminates electrons trapped in a metal sample (the "Compton effect" ). The energy of the light ($\gtrsim$ 10 keV) is sufficiently high that we can ignore the effect of the (small) workfunction of the metal ($\sim$ 1 eV), and the (small) kinetic energy of the electrons ($\lesssim$ 1 eV), and consider the electrons to all be free and at rest. The incoming X-rays, with wavelength $\lambda$, scatter from the electrons, causing the electrons to recoil. We measure the wavelength $\lambda'$ of the scattered X-rays as a function of the scattering angle $\theta$. We observe (see {numref}`fig:compton`) that $\lambda'$ depends on $\theta$, and is largest when $\theta = 180 ^{\circ}$, i.e. when the X-rays are scattered back in the direction that they came from.

By considering conservation of energy and momentum and using some special relativity we can derive an equation that explains this behaviour in the photon picture of light 
```{math}
:label: eqn1.4
\lambda' - \lambda = \frac{h}{m_ec}(1-\cos\theta),
```
where $m_e$ is the rest mass of the electron. When the X-rays are back-scattered with $\theta = 180^{\circ}$, they lose the maximum amount of energy possible ($2h/m_ec$), they obtain their lowest possible energy, and their wavelength is maximised (since $E_p = hc/\lambda$). In this case the electrons recoil with the maximum possible energy (equal to $2h/m_ec$ by conservation of energy). The constant quantity $h/m_ec$ is called the compton wavelength of the electron.

