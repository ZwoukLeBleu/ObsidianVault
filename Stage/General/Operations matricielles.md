### Transposition
Inverse une matrice.
Ex:
$$A = \begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix} \implies A^T=\begin{pmatrix}
1 & 3 \\
2 & 4
\end{pmatrix}$$
Et
$$B=\begin{pmatrix}
1 & 2 & 3
\end{pmatrix} \implies B^T=\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix}$$

### Conjugue complexe
Le conjugue complexe d'un nombre $C = a + bi$ est simplement $C^* = a - bi$. On inverse l’opérande de la partie complexe.

### Multiplication

### Produit scalaire

### Produit vectoriel

### Produit tensoriel
Aussi parfois appele le produit dyalique, il est dénoté par le symbole $\otimes$. Donc, $A\otimes B = C$ 
$$X = \begin{pmatrix}
1 \\
2
\end{pmatrix}\qquad
Y=\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix}$$
$$X\otimes Y = \begin{pmatrix}
x_0y_0 & x_0y_1 & x_0y_2 \\
x_1y_0 & x_1 y_1 & x_1y_2
\end{pmatrix}=\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6
\end{pmatrix}$$
$$Y\otimes X = \begin{pmatrix}
y_0x_0 & y_0x_1 \\
y_1x_0 & y_1x_1 \\
y_2x_0 & y_2x_1
\end{pmatrix} = \begin{pmatrix}
1 & 2 \\
2 & 4 \\
3 & 6
\end{pmatrix}$$
Pour des *vecteurs* $a,\ b$, le produit tensoriel peux être vu comme étant le produit matriciel entre $a$ et le transposé de $b$ tel que:
$$a\otimes b = a\cdot b^T$$


### Produit de Kronecker
![[Pasted image 20250904115951.png]]