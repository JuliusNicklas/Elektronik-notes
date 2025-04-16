Contains one voltage source, resistor, and [[Capacitor]].

For a first order RC-circuit we want to find time constant $\tau$, initial voltage $v_c(0) = 0$ and final voltage $v_c(\infty) = 1$.

**Step response:**
$v_c(t) = (1-e^{-1/\tau})u(t)$ (charge up)

**Current step response:**
$i_c(t) =\frac{1}{r}e^{-t/\tau}u(t)$ (charge up)

### Capacitor when $t \rightarrow 0^+$
(Initial condition)
Capacitor voltage must be continuous.
Capacitor acts as voltage source, 0 impedance.

### Capacitor when $t \rightarrow \infty$
(Final concition)
After $t > 5\tau$, the voltage is stable.
No current flows through.
It acts as an open circuit. (Infinite impedance)

### Last, put in equation:
$\tau = R_{Th}C$ from [[Thevenin's Theorem]]
$x(t) = ( x(\infty) +(x(0^+) - x(\infty))e^{-t/\tau} )u(t)$ [[u(t)]]
$x(t)$ can be either voltage or current over time.

### Steps for solution:
1. Find time constant $\tau = RC$
2. Find initial condition(s)
3. Find final condition(s)
4. Put in the equation

### Tips
If we have ramp function as input, we can take the derivative of the step function.


[[Laplace Transform]]

[[Basic components and circuit theory 3]]
[[Basic components and circuit theory 4]]
