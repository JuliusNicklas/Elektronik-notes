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

[[Elektronik data conversion]]