La *Internet Header Length (IHL)* est en chunks de 32 bits, soit 4 bytes. Il est, au minimum, là 5 fois.
Le type de service (?) est pour identifier la qualité du paquet, mais est souvent ignoré

### Taille maximal (16 bits, MTU)
La taille maximal d'un paquet IPv4 est de 64 kilobytes puisque la représentation est représenté par 16 bits. De ce, $2^{16} = 65536$

### DF (1 bit)
Dont Fragment
Si il est actif (=1), il dit au programme d'interdire la fragmentation de paquet.

### MF (1 bit)
More Fragment

### Fragment offset (13 bits)
Son unité est nécessairement un multiple de 8 bytes

### TTL (16 bits)
Détermine le nombre maximum de saut qu'un paquet peut faire
Fait en sorte qu'un paquet ne peut pas tourner en rond
Maximum de 255.
Il modifie l'entete

### Protocole (8 bits)
Assigne un protocol

### Header checksum (16 bits)
Fait juste dire si un paquet est bon ou non. Il ne sera pas transférée, ni corrigé.

> [!P.S]
> Le ICMP est un protocole d'envoie d'erreurs. Generalement, c'est ce qui est utilise avec IPv4


# Masques
Lorsqu'on prend une adresse IP et l'on applique un *&* logique par dessus (masque), on obtient l'adresse réseau.




