### Bobine 
- *Vert* = A
- ==Jaune== = B
- ***Blanc*** = C

- $0.78\cdot c = 2.34\cdot10^8m/s$ = vitesse de propagation


## Temporel
Le signal envoyé est une onde carré où $DC=50\%, f=1MHz, V_{pp}=10V$
$$\Delta x = t\cdot v$$

#### A --> B
'C' est sur la résistance

$\Delta t = 67.40ns$ entre impulsion 1 et reflection 1
$\implies 2.34\cdot10^8\cdot 67.40\cdot10^{-9}$
$$\Delta x\approx 15.7716m$$

#### A --> C
'B' est sur la résistance

$\Delta t = 58.00ns$ entre impulsion 1 et reflection 1
$\implies 2.34\cdot10^8\cdot 58.00\cdot10^{-9}$
$$\Delta x\approx 13.5720m$$

#### B --> C
'A' est sur la résistance

$\Delta t = 51.60ns$ entre impulsion 1 et reflection 1
$\implies 2.34\cdot10^8\cdot 51.60\cdot10^{-9}$
$$\Delta x\approx 12.0744m$$

### Résultats approximatif
$A + B +0C = 15.77$
$A + 0B+ C = 13.57$
$0A + B + C = 12.07$

Avec *Gauss-Jordan*, il est possible de trouver a, b et c :

| A   | B   | C   | $\Delta x$ |
| --- | --- | --- | ---------- |
| 1   | 1   | 0   | 15.77      |
| 1   | 0   | 1   | 13.57      |
| 0   | 1   | 1   | 12.07      |

$A = 8.6346m$
$B = 7.137m$
$C = 4.9374m$


## Fréquentielle
$$\hat{V}(z) = \hat{V}^+e^{-j\beta z} + \hat{V}^-e^{j\beta z}$$$$\hat{I}(z) = \dfrac{\hat{V}^+}{Z_c}e^{-j\beta z} - \dfrac{\hat{V}^-}{Z_c}e^{j\beta z}$$, où $\beta = \dfrac{\omega}{v}rads/m$

Ainsi que$$$$
