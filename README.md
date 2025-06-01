# Multi-Controlled-U-Gate
This is python code using only arbitrary 1-qubit and CX gates to create a Multi-controlled U gate
We use the ideas from Nielsen and Chuang, following the ideas of figure 4.10. 
The construction uses $n$ control qubits, $n-1$ ancillary qubits and $1$ target qubit.
In general, the construction costs $18n-12$ 1-qubit gates and $12n-10$ CNOT gates for this construction of one $C^n U$.
Our construction of $C^n U$ has circuit depth of $24n-17.$
