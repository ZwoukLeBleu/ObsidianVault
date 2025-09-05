### Etat du vide
Est l'etat initial d'un circuit ou tous les qubits sont dans l'etat $\ket{0}$. 
$$\ket{\mathbf{0}}=\ket{0}^{\otimes n}=\ket{0\dots00}$$
$$\ket{\mathbf{0}} = \begin{pmatrix}
1 \\
0 \\
\vdots \\
0
\end{pmatrix}$$

### Etat de superposition uniforme
Est caracteriser par le fait que toutes les possibilites du systemes on des chances egale.
$$\ket{+}^{\otimes n}$$
$$\ket{+}^{\otimes n}= \dfrac{1}{\sqrt{2^n}} \begin{pmatrix}
1 \\
1 \\
\vdots \\
1
\end{pmatrix}$$

### Etat GHZ
L'etat Greenberger-Horne-Zeilinger est un etat quantique enchevêtré (brouiller?) a au moins 3 qubits. Il fait intervenir 2 [[Etats de base]], un ou tout les qubits sont de $\ket{0}$, et un ou ils sont tous de $\ket{1}$. 
Pour un systeme de 3 qubits, il s'ecrit:
$$\ket{GHZ}= \dfrac{1}{\sqrt2}(\ket{000}+\ket{111})$$
Pour n qubits:
$$\ket{GHZ}= \dfrac{1}{\sqrt2}(\ket{0}^{\otimes n}+\ket{1}^{\otimes n})$$

### Etat W
L'etat Wolfgang Dur est un etat enchevetre a 3 qubits. Il est une combinaison d'etats ou seul 1 qubit est dans letat $\ket{1}$
$$\ket{W}= \frac{1}{\sqrt3}(\ket{001}+\ket{010}+\ket{100})$$
$$\implies \ket{W}= \frac{1}{\sqrt n}(\ket{0\dots01}+\ket{0\dots10}+\dots+\ket{1\dots00})$$
Circuit permettant de cree un etat W:
![[Pasted image 20250905105901.png]]
![[Pasted image 20250905105836.png]]

