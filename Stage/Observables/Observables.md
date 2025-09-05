Pour determiner le vecteur d'etat d'un qubit a partir d'uniquement des mesures, il nous faut trouver les coordonnees $x,y,z$ sur la [[Sphère de Bloch]].
![[Pasted image 20250905114628.png]]

### Coordonnee en y
Il ne faut que faire des mesures et de compter le nombre total, le nombre de fois que on obtient 1 et aussi 0. Avec ces informations et assez de *shots*, on peut estimer sur quel hemisphere de la sphere on se trouve. Si $n_1 >> n_0$, alors on peut dire que on est dans l'hemisphere sud, et vice-versa. Si $n_1 \approx n_0$, alors on est probablement pres de l'equateur.
La difference normalise est:
$$\dfrac{n_0-n_1}{n}$$

### Coordonnee en z
Puisque $z=\cos\theta$, il nous faut trouver $\theta$. 
L'equation de l'etat quantique est directement relier a $\theta$ avec son equation:
$$\ket{\psi} = \cos(\frac{\theta}{2})\cdot\ket{0} + e^{i\phi} \sin(\frac{\theta}{2})\cdot\ket{1}$$
Puisque on a beaucoup de mesures, on a les probabilites de l'etat quantique
$$p_\psi(0)=|\braket{0|\psi}|^2 = \cos^2(\frac{\theta}{2}) \qquad et\qquad p_\psi(1)=|\braket{1|\psi}|^2 = \sin^2(\frac{\theta}{2})$$
$$\cos^2(\frac{\theta}{2})-\sin^2(\frac{\theta}{2}) = \cos(\theta)$$
$$\implies p_\psi(0)-p_\psi(1) = z$$

## Observables
![[Pasted image 20250905130035.png]]
### Observable en $\hat{Z}$
$$z = p_\psi(0)-p_\psi(1) = |\braket{\psi|0}|^2-|\braket{\psi|1}|^2= \braket{\psi|0}\braket{0|\psi}-\braket{\psi|1}\braket{1|\psi}$$
$$\implies z=\braket{\psi|\hat{Z}|\psi}$$

$$x=\braket{\psi|\hat{X}|\psi}=\sin\theta\cos\phi$$

### Observable en $\hat{Y}$
$$y=\braket{\psi|\hat{Y}|\psi}=\sin\theta\sin\phi$$

### Observable en $\hat{I}$
$$\braket{\psi|\hat{I}|\psi}=1$$

## Estimation
### Coordonnee en z
$$p_\psi(0)\approx \frac{n_0}{n}\qquad et \qquad p_\psi(1)\approx \frac{n_1}{n}$$
$$p_\psi(0)-p_\psi(1) = z$$
$$\implies \frac{n_0}{n}-\frac{n_1}{n} = z$$

### Coordonnee en x
![[Pasted image 20250905130125.png]]
$$x = p_\psi(+)-p_\psi(-)$$

et 
$$x=\braket{\psi|X|\psi}=\braket{\psi|HZH|\psi}=\braket{\psi^{(x)}|Z|\psi^{(x)}}$$
lorsque $\ket{\psi^{(x)}}=H\ket{\psi}$


### Coordonnee en y
$$y = p_\psi(+i)-p_\psi(-i)$$
et
$$y=\braket{\psi|Y|\psi}=\braket{\psi|SXS^\dagger|\psi}=\braket{\psi|SHZHS^\dagger|\psi}=\braket{\psi^{(y)}|Z|\psi^{(y)}}$$
lorsque $\ket{\psi^{(y)}}=HS^\dagger\ket{\psi}$


### Reconstruction
Puisque c'est un estime, on n'aura pas nécessairement $x^2+y^2+z^2=1$.
$$\theta=\arccos z\qquad \qquad \phi=\arctan2(y,z)$$
$$\implies \ket{\psi}=\begin{pmatrix}
\cos(\frac{\theta}{2}) \\
e^{i\phi}\sin(\frac{\theta}{2})
\end{pmatrix}$$