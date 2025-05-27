---
tags:
  - Module3
aliases:
  - Inductors
---
# Inductance (L)
When forcing change in current flowing through wire it creates a reactive voltage by its magnetic field to oppose the change.

This voltage is called $V_L$
It does not produce current in the way a voltage source would, because it is simply opposing the stronger force which is creating the current. "It tries to produce current in the opposite direction of the current through the circuit, but is weaker"

The Electromotive force ($Emf$) opposes the change. Inductance (L) (measured in Henry (H)) of a conductior is the proportionality between $Emf$ and a given rate of change in current. 

$$
Emf = -L \frac {di} {dt}
$$
$$
V_L = L \frac {di} {dt}
$$

### Stored energy
When we feed increasing current into an inductor i it stores energy. When the current is ramped down, it discharges
Instantaneous power:$$
p_L(t) = v_L(t)*i_L(t)
$$
$$
V_L(t) = L \frac {di_L/t)} {dt} 
$$
![[Screenshot 2025-05-14 at 11.41.56.png]]

### Series inductors
ONE BIG INDUCTOR!
Sum of inductances

###  Parallel inductors
$$
\frac {1} {L_{eq}} =  \sum^N_{n=1} \frac {1} {L_n}
$$
[[Inductance and Steady State]]