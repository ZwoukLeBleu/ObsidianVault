## E1 (VPN//RPV)
### .1
On utilise AES & RSA pour la simple raison que si on n'aurait que AES, ca serait tres facile à briser, et si on aurait que RSA, ca serait trop long à chiffrer.

### .2

## E2
### a.
On peut faire l'operateur *modulo* peut importe ou dans l'equation (Dans ce cas ci-dessous, on l'a appliqué avant la mise au carré)
$$V=Kn+r$$
$$V^2\mod n \equiv r^2$$
### b.
Soit $T=UW, \qquad T,U,W \in \mathbb{Z}$


## E3
### a.
Sa complexité est nécessairement $O(n)=\sqrt{n}$ ou plus petit.

### b. 
Le cribe d'Erathosthene indique que pour trouver les nombres premier jusqu'a $N$, il faut:
1. Ecrire tout les nombres avant celui-ci
2. Pour chaque nombre, on le regarde, puis on enlève tout ses multiples (ex $2 \rightarrow \cancel{\{4,6,8...\}}$)
3. On repete jusqu'a $N$

### c. Miller-Rabin
$$a^{p-1}\equiv 1\mod p$$
$$\sqrt{2^{16}}\equiv\sqrt{1}\mod 17$$
$$2^8 \rightarrow 2^4 \rightarrow2^2\rightarrow2^1=1$$
$$\implies 2\mod 17 \rightarrow 4\mod 17 \rightarrow 8\mod 17 \rightarrow16\mod 17 \rightarrow$$
$$16\mod17\equiv -1\mod17$$
$$\implies 2^{16}\equiv1\mod 17$$
Si on a une transition d'un nombre autre que 1 vers 1, alors on est certain que le nombre est composé (pas premier). Cependant, si on n'a jamais de 1, alors il y a $\dfrac{1}{4}$ chance que ce soit un faux-positif.

### d. 
La distance moyenne pour un nombre premier $W$ est $ln (W)$.

Soit $n=30, \qquad 2x3x5$
Il reste alors $\{1,7,11,13,17,19,23,19\}$
Et $\dfrac{8}{30}\cdot\ln 512 \approx 100$
Donc, il y a en moyenne 1/100 nombre qui sont premier


## E4
### a.
$(g, p) \qquad x, y$\

*A* -------------- *B*
$g^x\mod p$ ---> *B*
*A* <--- $g^y\mod p$

=> $g^{xy}\mod p$



$$p=2_{p_1,p_2,p_3...p_{max}}+1$$
Si $p=2\cdot p_{max} + 1$, alors il est considere un nombre de Sophie Germain
$$|g|=p-1-2P_{max}$$
Dans Diffie-Hellman, $g,p,q(p_{max})$ peuvent etre publique, et seul $x,y$ doivent rester prive

1. $p,q$ doit etre premier
2. $1\equiv p\mod q$
3. $1\equiv g^q\mod p$

## E5
### a.
1. Non (1007)

### b.
1. OK
2. Non

### c.
1. Non (123471)

### d. 
1jai pas suivi

## E6
[[Methode p-1 de Pollard]]
essayer (fred croit que la reponse x=4)
Soit $n=482723$

$$2^1\mod 482723\equiv2\implies PGCD(n, 2-1)=1$$
$$(2^1)^2\mod 482723\equiv4 \implies PGCD(482723, 3)=1$$
$$((2^1)^2)^3\mod 482723\equiv64 \implies PGCD(482723, 63)=1$$
$$(((2^1)^2)^3)^4\mod 482723\equiv64^4 \implies PGCD(482723, (64^4\mod n)-1)=241$$

$$n=p\cdot q\implies p=\dfrac{n}{q}$$
$$\dfrac{482723}{241}=2003=p$$
