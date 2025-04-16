---
tags:
  - Module2
---

Map analog to digital amplitude.

Precision depends on resolution. 

### $N$ bit binary quantiser
Resolution of N bits, $2^N$ levels.
Analog signal $V_a$ between 0 and $V_{fs}$ 
Value of LSB: $\Delta = V_{LSB} = \frac{V_{fs}}{2^N-1}$ (Also the step between any 2 discrete levels )

### Quantisation error 
Also called quantisation noise and is similar to noise, but is not noise.

**When rounding:** 
Max quantisation error $Q_{max} = \Delta/2$
$\Delta = \frac{V_{fs}}{2^N-1}$

**When truncating:** 
Max quantisation error $Q_{max} = \Delta$
$\Delta = \frac{V_{fs}}{2^N}$

Max range of convertible analog signal $DR = V_{a,max}[dBV] - V_{a,min}[dBV]$ [[Logarithmic Scale (dB)]]
- $V_{a,max}[dBV]$: Limited by nonlinearities
- $V_{a,min}[dBV]$: Limited by quantisation error and thermal noise

### Gain function & error
**Gain function:**
A linear function from analog measurement $V_a$ to digital level $D$.
$D = G(V_a - V_{a0})$
In an ideal binary quantiser $G = 1/\Delta$ and $V_{a0}$.

**Gain error:**
Wrong G
(In binary quantiser: Wrong $\Delta = V_{LSB}$.)
- Gain Expansion $G > G_{ideal}$: 
	- Cannot capture higher analog levels
	- Limited range
- Gain Compression: $G < G_{ideal}$: 
	- Wasted bits
	- ???? larger Q ??????
	- ???? lower snr ????

**Offset error:**
Wrong offset $V_{a0} = \Delta_0$
Occurs when $\Delta_0 > V_{LSB}$
Can usually be corrected for if measured.


[[Elektronik data conversion]]