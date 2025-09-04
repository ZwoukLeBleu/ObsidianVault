Exemple classique: XOR $(x\oplus y)$ --> irreversible

## CNOT
Veux dire Controlled-NOT.
Est comparable a un XOR quantique reversible
$$CNOT = \begin{pmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0
\end{pmatrix} = |00X00| + |01X01| + |10X11| + |11X10|$$

EXEMPLES
$$CNOT\cdot\ket{00}_{xy} = CNOT\cdot\begin{pmatrix}
1 \\
0 \\
0 \\
0
\end{pmatrix} = \begin{pmatrix}
1 \\
0 \\
0 \\
0
\end{pmatrix} =\ket{00}_{xy} $$
$$CNOT\cdot\ket{10}_{xy} = \ket{11}_{xy}$$


#### Table de sortie

| INPUT  | OUTPUT           |
| ------ | ---------------- |
| x \| y | x \| $x\oplus y$ |
| 0   0  | 0   0            |
| 0   1  | 0   1            |
| 1   0  | 1   1            |
| 1   1  | 1   0            |

