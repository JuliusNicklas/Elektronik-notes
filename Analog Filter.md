---
tags:
  - Module3
---

[[Filter]] but Analog

# Why analog?
### [[Aliasing]]

AAF Filters must be low pass


### Noise Folding
/// White noise is uniform across all frequencies, and can therefore not be removed digita

Out-of-band noise 

### Image Folding
Need image rejecting filter (IRF) (Image Rejection Filter)
IRF filters must be band pass.

# Filter types
- Low pass – Only low frequencies pass
- High pass
- Band pass – Narrow band of frequencies pass
- Band stop – Stops a band

### Filter characteristics
![[Screenshot 2025-05-13 at 13.38.37.png]]

### Linear system math
Filters operate in the frequency domain.
$H(s)$ is the transfer function
$s = j\omega \rightarrow |H(j\omega)|$ This is the magnitude of the transfer function

$|V_{out(j\omega)}| = |H(j\omega)|\cdot|V_{in}(j\omega)|$ Amplitude out is original amplitude times filters magnitude

$H(s)=H(0)\frac{N(s)}{D(s)} \implies H(j\omega)=H(0)\frac{N(j\omega)}{D(j\omega)}$ This is just standard rational form. 

Phase shift: $\angle V_{out(j\omega)} = \angle H(j\omega) + \angle V_{in}(j\omega)$ angle here means phase of
$\angle H(j\omega) = arg N(j\omega) + arg D(j\omega)$
In this case phase shift is delay.
$\Delta t = \angle H(j\omega)/\omega$ To convert to time
^ This is derived from $\Delta t = \frac{..H..}{2\pi} \cdot T = \frac{..H..}{2\pi f} = \frac{..H..}{\omega}$

Remember zeroes and poles of transfer function.


For a low pass filter The frequency of the pole is equal to $(\tau 2\pi)^{-1}$


[[Analog Filters]]