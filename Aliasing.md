### Aliasing
Some signals with different frequencies can be sampled exactly the same. Only happens if $f_s$ is lower than Nyquist rate. For the highest of the signal frequencies $f_{sig}$ 

Aliasing of signal $f_{sig}$ happens att frequencies $f_n = n \cdot f_s \pm f_{sig}$.

Aliasing is problematic if some noise happens to fall on an alias frequency.

Aliasing of noise means more noise att lower frequencies.

### Anti-aliasing filtering
Must reject interference signals at $f > f_s - f_{sig}$
Must be analog.

Over sampling makes anti-aliasing easier
... More to write...

[[Elektronik data conversion]]