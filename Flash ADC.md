---
tags:
  - Module2
---

An [[ADC]]. A simple comparator.

Has 2 inputs: $V_{in}$ , $V_{ref}$
Returns 1 if $V_{in} > V_{ref}$

Can be made into a ladder with serial resistors to get many levels. If a ladder is made this way it outputs "thermometer code" (000, 001, 011, 111), a decoder is needed to convert it to 2's complement.

[[ADDA Circuits]]