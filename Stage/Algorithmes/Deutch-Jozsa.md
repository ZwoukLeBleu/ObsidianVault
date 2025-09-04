
Soit $f:\{0,1\}^n \rightarrow \{0,1\}$, realisé par un [[Oracle]], dont on sait que $f$ est constant ou balancé.

*But*: Determiner si $f$ est constant ou balancé.

Solution classique: 
	Il est nécessaire de demander a l'oracle *au moins deux fois*.
	Si l'on obtient deux réponses différente, on sait que $f$ est balancé
	Si l'on obtient deux fois la meme réponse, il faudra lui demander une autre fois, et encore, jusqu’à $2^{n-1}+1$ fois, ou $n$ est le # de bit en entree, 

Solution quantique:
	On n'a besoin de demander a l'oracle seulement que *une seule fois*!
	

### Circuit
![[Pasted image 20250903100734.png]]

Si la reponse total $y$ est egale a $00\dots0$, alors $f$ est constant. Autrement (si il y au moins un $1$), la fonction est alors balancé.

### Preuve
tente pas check ca a place
![[Pasted image 20250903101354.png]]

### Probabilité
#### Chaine de 0 $\ket{00\dots0}$
$$
\DeclarePairedDelimiter\abs{\lvert}{\rvert}
\DeclarePairedDelimiter\norm{\lVert}{\rVert}

P[y=00..0] = \abs*{\braket{00..0|\psi_3}}^2 = \abs*{\sum_{k\in [0,1]^n} C_k\cdot \braket{00..0|k}}^2 = \abs*{C_{00\dots0}}^2$$
$\implies \begin{Bmatrix}1,\quad k=00\dots0 \ \  \qquad\\0,\quad else\ (orthogonal)\end{Bmatrix}$
$$=\abs*{\frac{1}{2^n}\cdot\sum_{x\in[0,1]^n} (-1)^{f(x)}}^2
$$
$\implies \begin{Bmatrix} +2^n, \quad si\ f(x)=0\\ -2^n, \quad si\ f(x)=1 \\ 0, \quad si\ f(x)=bal.\end{Bmatrix}$


$$ \implies \begin{Bmatrix}
1, \quad si \ f(x)=constant \\
0, \quad si \ f(x)=balancé \ \
\end{Bmatrix}$$

??????????

je comprend pas! lol!


