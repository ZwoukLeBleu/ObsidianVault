Pour qu'une porte soit considere Hermitienne, la porte $P$ doit etre sont propre conjugue hermitien, cest a dire que $P=P^{\dagger}$. 
Une porte hermitienne appliqué deux fois sur un qubit redonnera toujours le meme etat, tel que
$$P_H\cdot P_H\cdot Q_b = Q_b$$

Le conjugue hermitien de $P$ est simplement la [[Operations matricielles#Transposition|transposition]] suivie du [[Operations matricielles#Conjugue complexe|conjugue complexe]] sur les elements de la matrice.
$$P^{\dagger} = (P^T)^*$$
Par exemple, soit 
$$Y = \begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix}$$
$$\implies Y^T = \begin{pmatrix}
0 & i \\
-i & 0
\end{pmatrix}$$
$$\implies (Y^T)^* = \begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix}$$
Donc, $Y$ est une matrice hermitienne, puisque $Y=Y^{\dagger}$ !
