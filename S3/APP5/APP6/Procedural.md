#### n
	$n=pq$
	$a^{p-1}=1\mod(p)$

#### e (encrypt)
e est nécessairement [[Coprime]] avec n
	$1<e<\phi(n)$
	

#### d (decrypt)
	$d\cdot e\mod(\phi(n))=1$

#### $\phi(n)$
	$\phi(n)=(p-1)(q-1)$
	$a^{\phi(n)}=1\mod(n)$


## E1
Soit $p=5, q=11$
### a.
$n=p*q = 55$

### b.
$e=59, d=?$
$\phi = 40$
$\implies 59\cdot d\mod(40)=1$

$\implies d = 19$
[[PGCD]]

### c.
Non, puisque si $e=2K$, alors le [[PGCD]] sera toujours au minimum *2*, (et non *1*!), ce qui fait que il n'y a pas d'inverse multiplicatif.


### d.
si $e=5,15,25,35, d=?$
$\implies 5\cdot d\mod(40)=1$
Dans le cas présent, puisque $(q-1)=10=5*2$, alors q est un multiple de 5. Il n'y aura donc pas de $e=5K$ satisfaisant.

### e.
Si $e=9,11,19,21,31\ ou\ 39$, est-ce que $d$ existe? 
Oui, $d$ existe et fonctionne pour tous, mais puisque $e<\phi(n), \implies d\equiv e$

### f.
skipped?

### h.
$e= (3,55)$
$d=(27, 55)$
Soit $m=30$, 

### j.
$54^3\mod(55)$
$54=55-1\implies [-1]^3$
$c=-1\equiv 54$

### k.
Soit $m=11,22,33$ et $(n,e)=(55,3)$
A voir semaine prochaine

### l.
pas fait.

## E2
Soit $x\in \mathbb{N}$,
	$0\equiv x\mod5$ ---> $7*11*13$
	$2\equiv x\mod7$ ---> $(5*11*13)*2$
	$1\equiv x\mod11$ ---> $5*7*13$
	$10\equiv x\mod13$ ---> $5*7*11$


| x=  | mod |           | mod equals | mutiply | total |
| --- | --- | --------- | ---------- | ------- | ----- |
| 0   | 5   | $7*11*13$ | 0          | 0       | 0     |
| 2   | 7   | $5*11*13$ | 1          | 2       | 1430  |
| 1   | 11  | $5*7*13$  | 4          | 3       | 1365  |
| 10  | 13  | $5*7*11$  | 8          | 5*10    | 19250 |
| -   | -   | -         | -          | -       | 22045 |
$22045\mod(5*7*11*13) \equiv 2025$


## E3
### a.
Soit $(n,e)=(86429, 5), \qquad p,q=? \qquad f(x)=x^2+5,\ x_0=1$ 
[[Méthode ρ de Pollard]]
$86429=p\cdot q$
$p<q$
$$|x_i-y_i|=K\cdot p, \qquad p\cdot q$$
$$\implies PGCD(|x_i-y_i|, n) = p$$

Alors, 

| Num | $x$     | $y$     | PGCD (!=1) |
| --- | ------- | ------- | ---------- |
| 1   | 6       | 41      | 7          |
| 2   | 41      | 2842601 |            |
| 3   | 1686    |         |            |
| 4   | 2842601 |         |            |
Donc, $p=7\implies \dfrac{86429}{7}=q\implies q=12347$


## E4
Soit $p=17$

### a. 
Soit $g=13$, combien de puissances distinctes de $g$ existes?
Il y a *4* valeurs distinctes

### b.
Voir colonne 8, et tout les $g\neq1$ sont bon.

### c.
Les cycles sont les multiples de $p-1$
Donc, ils sont de taille 1,2,4,8 et 16

## E5
A faire au procédural 2

## E6
#### n
$$(x-p)(x-q)=0$$
$$\implies x^2-qx-px+pq=0$$
$$\implies x^2-x(p+q)+pq=0$$

#### phi
$$(p-1)(q-1)=pq-(p+q)+1$$
$$= n-(p+q)+1$$

$$x^2+(\phi(n)-n-1)x+n=0$$
$$\implies p=331\qquad q=661$$







$$\implies \dfrac{x(p+q)\pm\sqrt{(-x(p+q))^2-4\cdot x^2\cdot pq}}{2x^2}$$

$$(-qx-px)(-qx-px)=q^2x^2+2pqx^2+p^2x^2=x^2(q^2+2pq+p^2)$$
$$\implies \dfrac{x(p+q)\pm\sqrt{x^2(q^2+2pq+p^2)-4\cdot x^2\cdot pq}}{2x^2}$$

