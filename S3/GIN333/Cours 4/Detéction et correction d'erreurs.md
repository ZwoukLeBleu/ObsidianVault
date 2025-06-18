### Erreurs
Accepter des erreurs est inacceptable.
Detecter les erreurs est essentiel.
Corriger les erreurs est optionnel.

On suppose que le message sera découopé en blocs *b* de *m* bits chacun, chaque bit étant tiré de l'ensemble $B = \{0,1\}$
Alors $b \in B^m = b_0, b_1, b_2 ... b_m-1, ou b_i \in \{0,1\}$
Supposons qu'on ajoute un bit $y\in B$ apres le bloc *b*, n dit qu’on a utilisé la fonction d’encodage f (b) = by
Une méthode usuelle est d’utiliser y comme bit de parité
pour b :
Si le nombre de 1 dans b est pair, alors y = 0
Si le nombre de 1 dans b est impair, alors y = 1
⇒ Si by a un nombre de 1 pair, alors il n’y a pas eu d’erreur
unique
⇒ Si by a un nombre de 1 impair, alors il y a eu une erreur


On suppose que le message est découpé comme dans
l’exemple précédent, en blocs b de m bits chacun
Supposons qu’on ajoute deux fois $B\in B^m$ après le bloc b.
On obtient un bloc codé *bbb*, la concaténation de trois
copies de *b*
On dit qu’on a utilisé la fonction de codage *f (b) = bbb*
