Les produits tensoriel ($\otimes$) sont utilise pour décrire les états multi-partie:
$$\ket{a} \otimes \ket{b} = \begin{pmatrix}
a_1 \\
a_2
\end{pmatrix}\otimes\begin{pmatrix}
b_1 \\
b_2
\end{pmatrix}
=\begin{pmatrix}
a_1 & b_1 \\
a_1 & b_2 \\
a_2 & b_1 \\
a_2 & b_2
\end{pmatrix}$$

Exemple: Système A est stable en $\ket{1}_A$ et B est stable en $\ket{0}_B$. L’état total (bipartite?) est alors $$\ket{10}_{AB} = \begin{pmatrix}
0 \\
1
\end{pmatrix}\otimes\begin{pmatrix}
1 \\
0
\end{pmatrix}
=
\begin{pmatrix}
0 \\
0 \\
1 \\
0
\end{pmatrix}$$
La taille du vecteur est de $2^q$, ou $q$ est le nombre de qubits impliqué/ dans l'operation.
> [!Note]
> Les états de cette forme sont appelé *non-corélé?*
> Les etats qui ne peuvent PAS etre ecrit de cette maniere ($\ket{\psi}_A\otimes\ket{\psi}_B)$ sont nommé des etats *corrélé*, et sont parfois aussi *emmelé (entangled)*

dwa