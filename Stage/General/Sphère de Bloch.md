Il est possible de décrire n'importe quel état normalise de la façon: $$\ket{\psi}=cos\frac{\theta}{2}\ket{0} + e^{i\phi} \cdot sin\frac{\theta}{2}\ket{1}$$
, ou $\theta$ est la probabilité de mesurer $\ket{0} \ket{1}$, et $\phi$ décrit la phase relative.

Tout etats pure peuvent etre illustre sur la surface d'une sphere de rayon de 1 (nommer Sphere de Bloch)


Les coordonees d'un tel etat sur la sphere sont :
$$\vec{r} = \begin{pmatrix}
\sin\theta \cos\theta \\
\sin\theta \sin\phi \\
\cos\theta
\end{pmatrix}$$



![[Pasted image 20250902122134.png]]

$$\ket{0}: \theta =0\quad \phi=arb. \implies \begin{pmatrix}
0 \\
0 \\
1
\end{pmatrix}$$
$$\ket{1}: \theta =\pi\quad \phi=arb. \implies \begin{pmatrix}
0 \\
0 \\
-1
\end{pmatrix}$$
$$\ket{+}: \theta =\frac{\pi}{2} \quad \phi=0 \implies \begin{pmatrix}
1 \\
0 \\
0
\end{pmatrix}$$
$$\ket{-}: \theta =\frac{\pi}{2} \quad \phi=\pi \implies \begin{pmatrix}
-1 \\
0 \\
0
\end{pmatrix}$$
$$\ket{+i}: \theta =\frac{\pi}{2} \quad \phi=\frac{\pi}{2} \implies \begin{pmatrix}
0 \\
1 \\
0
\end{pmatrix}$$$$\ket{-i}: \theta =\frac{\pi}{2} \quad \phi=\frac{3\pi}{2} \implies \begin{pmatrix}
0 \\
-1 \\
0
\end{pmatrix}$$

> [!caution]
> Les angles sur la sphere de Bloch sont deux fois plus grand que ceux dans l'[[espace Hilberteen]]! 
> Par exemple, $\ket{0}\ \&\ \ket{1}$ sont orthagonal dans Hilbert (90deg.), mais sont de 180deg. sur la sphere.

