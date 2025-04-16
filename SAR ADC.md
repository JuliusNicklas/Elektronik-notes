---
tags:
  - Module2
---

Successive Approximation [[ADC]]. Uses multiple cycles to compare voltage.

![[SuccApprADC.png]]
It tests by setting 1 bit at a time (left to right) to 1. If the total current number makes the [[DAC]] output a voltage higher than the input, it drops current bit to 0 and tries the next bit. 

It truncates the number, so the approximation is not necessarily the closest. 
SAR ADC is very good, very fast, very little power. Drawback is it takes time, few cycle.

[[ADDA Circuits]]
