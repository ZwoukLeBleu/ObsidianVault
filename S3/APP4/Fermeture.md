
# 7 - Application
### Sémantique
Apparence/manière d’interagir avec l'application


# 6 - Présentation
### Gestion de la syntaxe
Organisation des données. C'est uniforme pour tout les systèmes
- Compression
- Chiffrement


# 5 - Session
### Gestion du dialogue
- Ouverture
- Maintient
- Reprise
- Fermeture


# 4 - Transport
Unité de base: *messages, fragments*
Transfert les messages de bout-en-bout. Pour ce faire, il fait de la fragmentation et du réassemblage.
### Transfert
- [[TCP]], [[UDP]]
- [[IPv4|MTU]] (Maximum Transfer Unit)
- Multiplexage applicatif (série de fragments)
	- NAT / PAT


# 3 - Réseau
Unité de base: *paquet*
### Adressage
- Public/privé
- Physique ([[Adresse MAC|MAC]]) & logique ([[IPv4|IP]])
- Statique **V.S** dynamique (DHCP)
- Hiérarchique **V.S** absolue 

### Routage
- Interne ([[RIP]], [[OSPF]]) **V.S** externe (BGP)
- Statique (route) **V.S** dynamique (protocole)
- Proactive (Anticipation de route) **V.S** réactif
- Protocole (communication) **V.S** algorithme ()
- Vecteur de distance **V.S** vecteur d'état des liens


# 2 - Liaison de donnees
Unité de base : *trame*
### Trammage
- Préambule
- Chapeaux de début/fin (PPP)

### Control d’accès au support de transmission
- [[Division de transmission]]
- [[CSMA]]

### Control d'erreur
- [[Erreurs]]
- CRC (Ethernet: 32bits, PPP: 16bits)


# 1 - Physique
Unité de base : *bit*
### Types de support:
- Métallique: [[Cuivre]], aluminium, alliages 
- [[Fibre Optique]]
- [[Sans-fil]]

### Cablage structure:
- Vertical ([[Fibre Optique]])
- Horizontal ([[Cuivre]])

### Codage en ligne:
- [[Représentation de bit]]
- [[Mode de transfers]]
- [[Modulation]]




