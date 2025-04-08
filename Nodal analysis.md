
### Procedure
1. Simplify circuit
	- Remove resistance in *series* with current sources or in *parallel* with voltage sources
	- Replace Voltage sources with [[Norton's Equivalent Circuit|Norton]] equivalent 
2. Determine the Ground
	- Choose node with maximum connected branches
3. Wrote equation system in matrix form
	- Gauss elimination!! WOO!!
	- Circuit with $n$ nodes: $n$ equations and n independant voltages. (GND is 0)
	- $GV = I$ where G is the conductance matrix ($n$x$n$), V is the voltage vector and $I$ is the constant vector (R, V, -I, I). 
	- In $I$: $-$ if the current leaves the node and $+$ if it enters

[[Basic components and circuit theory 2]]
[[Basic components and circuit theory 3]]