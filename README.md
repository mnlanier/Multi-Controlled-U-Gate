# Multi-Controlled-U-Gate
This is python code using only arbitrary 1-qubit and CX gates to create a Multi-controlled U gate.
We use the ideas from Nielsen and Chuang, following the ideas of figure 4.10. 
The construction uses $n$ control qubits, $n-1$ ancillary qubits and $1$ target qubit.
In general, the construction costs $18n-12$ 1-qubit gates and $12n-10$ CNOT gates for this construction of one $C^n U$.
Our construction of $C^n U$ has circuit depth of $24n-17$.
The main function "MCU" has four inputs:
1: $n$, the number of control qubits
2: Theta, see below
3: Phi, see below
4: Lambda, see below

Theta, phi and lambda are the variables that define an arbitrary 1-qubit gate, defined as below:
$U(\theta, \varphi, \lambda)=$ 
```math \begin{bmatrix} \cos \left( \tfrac{\theta}{2} \right) & - e^{i \lambda} \sin \left( \tfrac{\theta}{2} \right) \\ e^{i \varphi} \sin \left( \tfrac{\theta}{2} \right) & e^{i (\varphi + \lambda)} \cos \left( \tfrac{\theta}{2} \right) \end{bmatrix}

