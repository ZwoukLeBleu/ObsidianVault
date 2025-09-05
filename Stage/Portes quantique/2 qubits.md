Une porte quantique a deux qubits modifie 2 qubits. Puisque les systemes a deux qubits sont definit par 4 [[Etats de base#2 qubits|vecteurs de base]], alors toute porte sera 2 qubits sera une matrice 4x4


## Portes controllées 


### CNOT (Controle-X)
Exemple classique: XOR $(x\oplus y)$ --> irreversible
Veux dire Controlled-NOT.
Est comparable a un XOR quantique reversible
$$CNOT = \begin{pmatrix}
1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0
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


#### Table de sortie

| INPUT  | OUTPUT           |
| ------ | ---------------- |
| x \| y | x \| $x\oplus y$ |
| 0   0  | 0   0            |
| 0   1  | 0   1            |
| 1   0  | 1   1            |
| 1   1  | 1   0            |

### Controle-Z
Cette porte applique au qubit cible la porte [[1 qubit#Z|Z]] si le qubit controle est $\ket{1}$, mais ne fait rien si le controle est en $\ket{0}$. Cependant, puisque la porte Z na pas deffet si le qubit affecté est en $\ket{0}$, alors, cette porte agit seulement si le systeme est au total en $\ket{11}$!
$$C\hat{Z} = \begin{pmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & -1
\end{pmatrix}$$

### SWAP
Pour echanger des qubits, puisque le systeme doit necessairement etre [[Unitaire]], alors cela doit se passer uniquement entre 2 qubits, d'ou vien la porte SWAP. Elle n'affecte rien si le systeme est $\ket{00}$ ou $\ket{11}$ car les 2 qubits sont identique, mais va interchanger $\ket{01}$ et $\ket{10}$.
$$SWAP= \begin{pmatrix}
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1
\end{pmatrix}$$
Trivia? : Une porte SWAP cest basically 3 CNOT ca a l'air
![[Pasted image 20250904145917.png]]


