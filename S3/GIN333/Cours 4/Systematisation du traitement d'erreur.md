Soit la fonction de codage $f: B^m \rightarrow B^n$
On suppose que *m < n*
*f* donne une image unique $c_b$ pour chaque *f(b)* (Pourquoi doit-elle etre unique?)
	- Certains codes n'existent pas dans Bn
	- Si un code reçu ne correspond pas à un code existant, alors il y a eu une erreur de transmission
On suppose alors que le code le plus "proche" est le bon, et on peut ensuite le decoder
On définit la proximité entre deux codes par le nombre de bits différents entre les deux codes
Pour calculer la distance : on effectue le ou-exclusif (bit
par bit) entre les deux codes
On calcule ensuite le nombre de 1s du résultat (on appelle
ce calcul la distance de Hamming D)

### Exemples: 
soit 
$c_1 = 0111, c_2 = 1110$
$c_1\oplus c_2$

Puisque b ∈ Bm et cb ∈ Bn, alors la distance minimale entre les codes cb ne peut dépasser n − m + 1, soit au maximum n − m codes libres (espaces) entre deux codes cb
$b\in \{00,01,10,11\},$
$f(b) \in \{000,011,101,110\}$, (*que fait f(b)?*)
![[kevin the cube.png]]
Si la distance minimale entre deux codes est t, alors on
peut détecter t − 1 erreurs dans Bn



Soit la fonction de codage $f: B^m \rightarrow B^n$
On dit que cette fonciton produit un code lineaire si limagede f dans Bn est un [[Sous-groupes]] de Bn

Le groupe $B_n$ est defini avec loperateur $\oplus$ (XOR)
Comment verifier que limage de f dans $B_n$ est un sous-groupe de $B_n$?
- On associe XOR a l'addition
- Element neutre: $0_n$ represente l'element de Bn qui ne contient que des zeros
- Inverse: Chaque element *u* de $B_n$ est son propre inverse ($u \oplus u = 0_n$)
- Associativité : $\oplus$ est associatif (c’est analogue à une addition)
- Fermeture : Pour que l’image de f soit un sous-groupe de $B_n$ , il suffit de démontrer que si u et v font partie de l’image de f dans $B_n$, alors ($u \oplus v$) fait aussi partie de l’image de f dans $B_n$


soit $f: B^m \rightarrow B^n$ un code lineaire
La distance minimale *D* entre 2 codes est le poids le plus faible des elements de l'image *f* a l'exeption du code 0n
- Soit $d = D(u \oplus v)$ la distance minimal entre les codes produits par f
- Soit *x* le poids minimal des elementss non-nuls de l'image issue de f, qui savere pour lelement *w*
- Puisque *w* et 0n sont des 

### Comment obtenir $f: B^m \rightarrow B^n$ ?
On definit la matrice generatrice *G* de la facont suivante:
Les elements de $G\in\{0,1\}$
G est une matrice m x n
- m est le nombre de bits du bloc message de départ b
- n  est le nombre de bits du code obtenu
G est composée d’une matrice identité m × m (Im), à laquelle on adjoint une matrice A de taille m × (n − m) : G = ImA, par exemple:
![[Pasted image 20250617100250.png]]


arrange toi 
![[Pasted image 20250617100632.png]]