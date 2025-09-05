$\mathbb{Z}_n$, ou $\mathbb{Z}/n\mathbb{Z}$ représente les classes d'equivalence de nombre entier, modulo $n$.

Soit $p$ un nombre premier:
- Pour la multiplication $\mod p$, la classe d'equivalence de..
	- \[0\] représente l'élément absorbant
	- \[1\] représente l'élément neutre
- Toutes les classes d'équivalence de $\mathbb{Z}^*_p$ sont relativement premieres avec $p$
- Les éléments de $\mathbb{Z}^*_p$ forment un [[Groupes Cycliques|groupe]] pour la multiplication

$\mathbb{Z}^*_p$ est un groupe si chacun de ses elements a un inverse:
- Soit $a \in \mathbb{Z}^*_p$. Supposons que $1<= a <= (p-1)$
- Supposons que $k$ est l'ordre de $a : a^k \equiv 1\mod p$
- Alors les nombres $1,a,a^2...a^{k-1} \mod p$ forment un [[Sous-groupes]] de $\mathbb{Z}^*_p$
- Selon le théoreme de Lagrange :
	 $k$ doit etre un facteur de $p-1$
	 Alors $km=p-1$, pour un certain nombre $m$
- D'ou $a^{p-1} \equiv a^{km} \equiv (a^k)^m \equiv 1^m \equiv 1\mod p$
- Et $a^{p-1} \equiv a\cdot a^{p-2} \equiv 1\mod p$
---> L'inverse multiplicatif $a^{-1} \mod p$ de $a$ existe et est toujours equivalent à: $a^{p-2}\equiv a^{k-1} \mod p$

Donc, $\mathbb{Z}^*_p$ est un groupe!

Selon le theoreme de Cauchy, il existe un $g$ dont l'ordre est $p-1$, alors $\mathbb{Z}^*_p$ est un groupe cyclique.



Soit $p=5$
$\mathbb{Z}^*_5=\{[1],[2],[3],[4]\}$
$\implies \mathbb{Z}^*_5 = \{1,2,3,4\}$

Selon Lagrange, puisque $|\mathbb{Z}^*_5| = 4$, il devrait y avoir des elements de cycles de taille 1,2 et 4:
	Puissance de *1* = {1}  -----------> Taille 1
	Puissance de *2* = {2,4,3,1}  -----> Taille 4
	Puissance de *3* = {3,4,2,1}  -----> Taille 4
	Puissance de *4* = {1, 4} ou {1, -1} -> Taille 2




Soit $n=p\times q$, ou $p,q$ sont premier
$G=\{[0], [1], [2]... [n-1]\}$?
Les trois premieresconditions sont satisfaites (fermeture, associativité,
élément neutre)
Qu’en est-il de l’existence d’un inverse pour chacun des
éléments du groupe ?
→ Il faut retirer [0]
→ Il faut retirer tous les multiples de p et q de l’ensemble G,
parce qu’ils n’ont pas d’inverse :
→ Pour que a ait un inverse modulo n, il faut que
PGCD(a, n) = 1, alors que PGCD(kp, n) = p 6 = 1

Au depart, $|G| = p\times q$
- On retire \[0\], alors il reste $p\times q-1$ elements
- On retire les facteurs de $p$, il y en a $q-1$
- On retire les facteurs de $q$, il y en a $p-1$
$$|G| = pq-1-(q-1)-(p-1)$$
$$\implies |G| = (p-1)(q-1)$$

Appelons $\mathbb{z}^{\phi (n)}_n$ cet ensemble $G$
On peut alors reprendre le raisonement utilise pour le petit theoreme de Fermat:
- Soit $a\in \mathbb{z}^{\phi (n)}_n, 1 <=a<=(n-1)$, ou $a\in [a] \mod a$ 
- Supposons que $k$ est l'ordre de $a:a^k\equiv 1\mod n$
- Alors les nombres $1, a, a^2... a^{k-1} \mod n$ forment un sous-groupe de $\mathbb{z}^{\phi (n)}_n$
- ????????


La methode de Miller-Rabin est basee sur le petit theoreme de Fermat:
- $a^{p-1} \equiv 1 \mod p$, alors $a\dfrac{p-1}{a}\equiv \sqrt{1}\mod p$
- Quelles sont les valeurs possible de $\sqrt{1} \mod p$
	- On desire : $x^2 \equiv 1 \mod p$
	- $x^2-1\equiv 0 \mod p$
	- $(x-1)(x+1) \equiv 0 \mod p$
	- Soit $y=x-1$ et $z=x+1$
		- Puisque $p$ est premier, il n'y a aucun facteurs plus petit que lui-meme
			--> 
		- $x_1\equiv 1\mod p$ et $x_2 \equiv -1\mod p$ sont les duex seules solutions.
	- De ce, $\sqrt{1}\equiv \{1,-1\}\mod p$ *!!!!!!!!!!!!!!!!!!!!!!!!!!!!*

On desire $x^2\equiv 1\mod n$
$x^2-1\equiv 0\mod n$
$(x-1)(x+1)\equiv 0\mod n$
Soit $y = x-1, \quad z=x+1$, on cherche $yz\equiv 0\mod n$

Si $y=k_1p, \quad z=k_2q$ :
	![[Pasted image 20250722135206.png]]
	

Soit $n=15$
$x_1=\sqrt{1}=1, \qquad x_2=\sqrt{1}=-1\equiv 14 \mod 15$ sont des solutions

Les autres solutionssont: 
	$x_3\equiv 1\mod 3, \qquad x_3\equiv -1\mod 5$
	$x_4\equiv -1\mod 3, \qquad x_4\equiv 1\mod 5$
fuck of
![[Pasted image 20250722135552.png]]


# Exercices
## E1 - $\mathbb{Z}^*_{13}$
### 1 - Taille de $\mathbb{Z}^*_{13}$
?
![[Pasted image 20250722141240.png]]


## E2 $n_1=111, \quad n_2=105$
### 1
$111=3\cdot37,\quad 105=3\cdot 35$
$(x+1)(x-1)$????????????????????

$x=37\mod 3 \implies x=3\mod37$
$1=37+(-12)\cdot 3 \mod 37$
$x=3\cdot(12$
wtf??
aqzswxde3c4frv5gtbhy6n7ujm8ik9,ol0.p;-/['=}|
]

