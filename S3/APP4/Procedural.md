## [[Modèle OSI]]

| COUCHE               | FONCTION                                                       | AUTRES        |
| -------------------- | -------------------------------------------------------------- | ------------- |
| Application          | Sémantique                                                     |               |
| Presentation         | Syntaxe                                                        |               |
| Session              | Dialogue (Ouverture, fermeture, maintien, reprise de session)  |               |
| Transport            | Segments/Fragments (Fragmentation, réassemblage, multiplexage) | Port          |
| Réseau               | Paquets (Adressage et routage)                                 | IP<br>Routeur |
| Liaison (de données) | Trammage (Structure les bits en trames)                        | MAC<br>Switch |
| Physique             | Envoie les bits physiquement                                   | Répéteur      |


## [[Modèle TCP-IP]]

| COUCHE      | PROTOCOLES      | ANALOGUE À  |
| ----------- | --------------- | ----------- |
| Application | HTTP, SMTP, FTP | OSI {7,6,5} |
| Transport   | TCP & UDP       | OSI {4}     |
| Internet    | IPv4/IPv6       | OSI {3}     |
| Accès       | ...?            | OSI {1,2}   |


[[Topologie]]
[[Area Networks]]


Dans un LAN Ethernet, la transmission se fait:
- Serie
- Synchrone
- Half-Duplex
- a


## 8.
Probabilité est unifirme dans l'intervalle $0\leq n < 2^n$
Le temps de transmission est lié au débit par rapport à la taille du paquet
$$t_{tn}=\dfrac{L+H}{D}$$
,ou L = donnees, H = entete, D= Debit
$t_p=\dfrac{d}{v_p}$

## 9.
> [!Info]
> J'ai pas suivi

## 10.


Avec les VLANs, il est possible d'avoir une [[Topologie]] physique maillé (ou n'importe quoi), mais qui est logiquement routé en forme d'arbre ou autre.


