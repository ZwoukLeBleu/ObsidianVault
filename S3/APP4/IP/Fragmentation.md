Soit un paquet de 3000 bytes qui doit être transféré avec un *Maximum Transfer Unit (MTU)* de 576, via [[IPv4]].
$$\dfrac{3000-20}{576-20} \implies 6 fragments$$
$576-20=556\implies552$ est le multiple de 8 le plus pres de 556. 

| Length | ID  | MF  | Offset |
| ------ | --- | --- | ------ |
| 552    | 123 | 1   | 0      |
| 552    | 123 | 1   | 69     |
| 552    | 123 | 1   | 138    |
| 552    | 123 | 1   | 207    |
| 552    | 123 | 1   | 276    |
| 220    | 123 | 0   | 345    |

