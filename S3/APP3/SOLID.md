### S - Single Responsibility
*Toutes fonctions n'ont qu'une seule tâche à accomplir*
Des petites fonctions qui n'effectue qu'uniquement une seule tache

### O - Open/Closed
*Ouvert à l'extension, fermé à la modification*
Pour changer une classe, il est plus pertinant de faire de l'héritage au lieu de modifier la classe mère, puisque faire pourrais causer des problèmes par rapport au autres méthodes qui utilise la classe mère.

### L - Liskov's Substitution
*Un enfant peut toujours remplacer sont parent*
Dans le fond, c'est le principe de polymorphisme

### I - Interface Segregation
*Chaque interfaces doivent êtres les plus petite possible*

### D - Dependency Inversion
Un parent n'a pas les caractéristiques d'un enfant (il ne peut pas garantir une méthode incomplète). Cependant, un enfant est certain d'avoir un parent.
