***not the same as [[Sound energy density|sound energy density]]***

sound pressure or acoustic pressure is the local pressure deviation from the ambient (average or equilibrium) atmospheric pressure, caused by a sound wave. 

in air, sound pressure can be measured using a  microphone, and in water with a hydrophone. The SI unit of sound pressure is the [[Pascal (unit)|pascal (Pa)]].

## Mathematical definition
---
a sound wave in a transmission medium causes a deviation (sound pressure, a *dynamic* pressure) in the local ambient pressure, a *static* pressure.

sound pressure, denoted $p$, is defined by

$$
p_\text{total} = p_\text{static} + p,
$$
where

- $p_\text{total}$ is the total pressure,
- $p_\text{static}$ is the static pressure.

### [[Sound intensity|sound intensity ]]

in a sound wave, the complementary variable to sound pressure is the [[Particle velocity|particle velocity]]. together, they determine the sound intensity of the wave.

sound intensity, denoted $\text{I}$ and measured in $\text{W}*\text{m}^-2$ in SI units, is defined by

$$
\text{I} = p\text{v}
$$
where 

* $p$ is the sound pressure,
* $\text{v}$ is the particle velocity

### [[Acoustic impedance|acoustic impedance]]

acoustic impedance, denoted $\text{Z}$ and measured in $\text{Pa}*\text{m}^-3*\text{s}$ in SI units, is defined by

$$
\text{Z}({s})=\frac{\widehat{p}(s)}{\widehat{Q}(s)},
$$
where
- $\widehat{p}(s)$ is the [[Laplace transform]] of sound pressure,
- $\widehat{Q}(s)$ is the Laplace transform of sound volume flow rate.

specific acoustic impedance, denoted $\text{z}$ and measured in $\text{Pa}*\text{m}^-1*\text{s}$ in SI units, is defined by

$$
\text{z}(s)=\frac{\widehat{p}(s)}{\widehat{v}(s)},
$$
where
- $\widehat{p}(s)$ is the Laplace transform of sound pressure,
- $\widehat{v}(s)$ is the Laplace transform of particle velocity.

### [[Particle displacement|particle displacement]]

the particle displacement of a *progressive [[Sine wave|sine wave]]* is given by

$$
\delta(r, t)=\delta_m\cos(k*r-\omega t+\varphi_{\delta,0}),
$$
where
- $\delta_m$ is the [[Amplitude|amplitude]] of the particle displacement. 
- $\varphi_{\delta,0}$ is the [[Phase shift|phase shift]] of the particle displacement,
- $k$ is the [[Wave vector|angular wave vector]],
- $\omega$ is the [[Angular frequency|angular frequency]].

it follows that the particle velocity and the sound pressure along the direction of propagation of the sound wave $x$ are given by

$$
\begin{align}
v(r,t)&=\frac{\partial\delta}{\partial t}(r,t)=\omega\delta_\text{m}\cos(k*r-\omega t+\varphi_{\delta,0}+\frac{\pi}{2})=v_\text{m}\cos(k*r-\omega t+\varphi_{v,0}), 
\\
\\
p(r,t)&=-\rho c^2\frac{\partial\delta}{\partial x}(r,t)=\rho c^2k_x\delta_\text{m}\cos(k*r-\omega t+\varphi_{\delta,0}+\frac{\pi}{2})=p_\text{m}\cos(k*r-\omega t+\varphi_{p,0}),
\end{align}
$$

where
- $v_m$ is the amplitude of the particle velocity,
- $\varphi_{v,0}$ is the phase shift of the particle velocity,
- $\rho_\text{m}$ is the amplitude of the acoustic pressure,
- $\varphi_{p,0}$ is the phase shift of the acoustic pressure.

taking the Laplace transforms of $v$ and $p$ with respect to time yields

$$
\begin{align}
\widehat{v}(r,s)&=v_\text{m}\frac{s\cos\varphi_{v,0}-\omega\sin\varphi_{v,0}}{s^2+\omega^2},
\\
\\
\widehat{p}(r,s)&=p_\text{m}\frac{s\cos\varphi_{p,0}-\omega\sin\varphi_{p,0}}{s^2+\omega^2},
\end{align}
$$

since $\varphi_{v,0}=\varphi_{p,0}$ , the amplitude of the specific acoustic impedance is given by

$$
\text{z}_\text{m}(r,s)=\lvert{z(r,s)}\rvert=\left|\frac{\widehat{p}(r,s)}{\widehat{v}(r,s)}\right|=\frac{p_\text{m}}{v_\text{m}}=\frac{\rho c^2k_x}{\omega}.
$$

consequently, the amplitude of the particle displacement is related to that of the acoustic velocity and the sound pressure by

$$
\begin{align}
\delta_\text{m}&=\frac{v_\text{m}}{\omega},
\\
\\
\delta_\text{m}&=\frac{p_\text{m}}{\omega z_\text{m}(r,s)}.
\end{align}
$$
### [[Inverse-square law|inverse proportional law]]

when measuring the sound pressure created by a sound source, it is important to measure the distance from the object as well, since the sound pressure of a spherical sound wave decreases as $1/r$ from the center of the sphere and not as $1/r^2$, like the sound intensity.

$$
p(r)\propto\frac{1}{r}.
$$

this relationship is an inverse-proportional law. 

if the sound pressure $p$