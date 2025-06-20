
### Proactif vs Reactif
*Proactif:* Prevoir la route avant meme de recevoir une requete
*Reactif:* Donner la route seulement lorsqu'on la demande

> [!Note]
> Lorsqu'un [[Équipement|routeur]] recoit un paquet contenant une addresse [[IPv4|IP]] inexistante, il décrémente son TTL et l'envoie à l'adresse par défault


### Distance Vector
Les protocoles à vecteur de distance, comme [[RIP]] partagent les informations de routage uniquement avec leurs voisins directement connectés, en s'appuyant sur des mises à jour itératives pour créer une image du réseau

### Linked State
remplie le réseau avec des informations sur leurs liens directement connectés, permettant à chaque routeur de construire une carte de la topologie complète du réseau et de calculer les itinéraires optimaux.