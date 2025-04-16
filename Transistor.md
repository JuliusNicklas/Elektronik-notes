---
tags:
  - Module2
---

A transistor is a form of electric [[Switch]]
### Mosfet
Mosfet - metal oxide semiconductor field effect transistor

Two parts: gate(metal) and body (doped [[Semiconductor]]), separated by oxide layer (undoped [[Semiconductor]]). 
When voltage is applied to the gate it pushes or pulls electrons in the body, which increases or decreases conductivity. 
With electrons clumping close to the gate, in the body, it creates a channel.
NMOS (p-type doping) or PMOS (n-type doping) changes if positive or negative voltage allows for channeling. NMOS is active with positive voltage. PMOS is active with negative voltage.
A transistor has 4 pins: B, Source, Gate, Drain.

Finfet - fin field effect transistor

# Mosfet for logic gates

... much to write ...
### Error
(Actually not gate, not transistor)
Ideal transistor lets through $V_{DD}$ when  $V_{in} < V_{DD}/2$ and $0V$ otherwise.
It is not ideal -> error/noise.
The transistor has max voltage output $V_{OH} < V_{DD}$ when $V_{in} < V_{IL} < V_{DD}/2$ and minimum voltage $V_{OL} > 0$ when $V_{in} > V_{IH} > V_{DD}/2$
When $V_{in} \approx V_{DD}/2$ the output is in the *linear* stage, and the output is somewhere in the middle, X.
We call high voltage 1, unknown voltage X, and low voltage 0.






[[Active Components (lecture)]]