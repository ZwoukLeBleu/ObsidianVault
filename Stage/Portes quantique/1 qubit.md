Exemple classique: NOT gate
Exemple quantique: Puisque la theory quantique est [[Unitaire]], alors les portes quantiques sont représenter par des matrices unitaires: $u^+u=ident.$

En [[Braket notation|notation de Dirac]]: $$u = \begin{pmatrix}
u_{00} & u_{01} \\
u_{10} & u_{11}
\end{pmatrix} = u_{00}|0X0|$$
Les portes $\sigma_x,\ \sigma_z,\ \sigma_y$ sont des *Pauli matrices*. Elles sont caractérisé par le fait que pour tout${\sigma_{.}}^2 = Ident. = \begin{pmatrix}1 & 0 \\0 & 1\end{pmatrix}$
Ensemble, avec la matrice identite, forment une base de matrices 2x2



## X (Bit flip)
Est equivalent a une [[Rotation sur Bloch#Rotation sur l'axe des X]] avec un angle de $\pi$

Est l'equivalent de la porte NOT du monde classique. Transforme un état $\ket{0}$ en $\ket{1}$, mais fonctionne aussi pour tout autre état. 
Correspond a une rotation de $\pi$ a l'entour de l'axe des X. 
$$X = \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}=|0X1|+|1X0|$$

#### Multiplication matricielle
$$\implies X\cdot\ket{0}=\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}\cdot\begin{pmatrix}
0 \\
1
\end{pmatrix}=\begin{pmatrix}
1 \\
0
\end{pmatrix}$$
$$=\ket{1}$$

#### Multiplication via Dirac
$$\sigma_x\cdot\ket{1}=(|0X1| + |1X0|)\cdot\ket{1}$$
$$=\ket{0}\braket{1|1}+\ket{1}\braket{0|1} = \ket{0}\cdot1+\ket{1}\cdot0$$
$$=\ket{0}$$

## Y
Est equivalent a une [[Rotation sur Bloch#Rotation sur l'axe des Z]] avec un angle de $\pi$

Correspond a une rotation de $\pi$ a l'entour de l'axe des Y
$$Y=\begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix} = i\cdot\sigma_x\cdot\sigma_z$$


## Z
Est equivalent a une [[Rotation sur Bloch#Rotation sur l'axe des Z]] avec un angle de $\pi$

Correspond a une rotation de $\pi$ a l'entour de l'axe des Z. 
$$Z = \begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix}=|0X0|-|1X1|$$

#### Multiplication matricielle
$$\implies \sigma_z\cdot\ket{+}=\begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix}
\cdot
\frac{1}{\sqrt2}\begin{pmatrix}
1 \\
1
\end{pmatrix}
=\frac{1}{\sqrt2}\begin{pmatrix}
1 \\
-1
\end{pmatrix}$$
$$=\ket{-}$$

#### Multiplication via Dirac
$$\sigma_z\cdot\ket{-}=(|0X0| - |1X1|)\cdot\ket{-}$$
$$\frac{1}{\sqrt2}(\ket{0}+\ket{1})$$
$$=\ket{+}$$



## S
Ajoute 90deg. a la phase $\phi$. Semble etre une demi porte Y.
$S\cdot H$ est applique pour changer de la base Z a Y

$$S = \begin{pmatrix}
1 & 0 \\
0 & i
\end{pmatrix}$$

## H (Hadamard)
Transforme les états $\ket{0}$ en $\ket{+}$, et $\ket{1}$ en $\ket{-}$, et vice-versa.
Generalement, cette porte créé les superpositions (initial) des qubits.
$$H = \frac{1}{\sqrt2}\begin{pmatrix}
1 & 1 \\
1 & -1
\end{pmatrix} = \frac{1}{\sqrt2}(|0X0| +|0X1| + |1X0| - |1x1|)$$

#### Multiplication matricielle
$$H\cdot \ket{0} = \frac{1}{\sqrt2}\begin{pmatrix}
1 & 1 \\
1 & -1
\end{pmatrix} \cdot \begin{pmatrix}
1 \\
0 
\end{pmatrix} = \frac{1}{\sqrt2}\begin{pmatrix}
1 \\
1 
\end{pmatrix}$$
$$=\ket{+}$$

