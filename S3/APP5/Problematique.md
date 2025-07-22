### Bobine 
- *Vert* = A
- ==Jaune== = B
- ***Blanc*** = C

- $0.66\cdot c = 1.98\cdot10^8m/s$ = vitesse de propagation


## Temporel
Le signal envoyé est une onde carré où $DC=50\%, f=1MHz, V_{pp}=10V$
$$\Delta x = t\cdot v$$

#### A --> B
'C' est sur la résistance

$\Delta t = 67.40ns$ entre impulsion 1 et reflection 1
$\implies 1.98\cdot10^8\cdot 67.40\cdot10^{-9}$
$$\Delta x\approx 13.3452m$$

#### A --> C
'B' est sur la résistance

$\Delta t = 58.00ns$ entre impulsion 1 et reflection 1
$\implies 1.98\cdot10^8\cdot 58.00\cdot10^{-9}$
$$\Delta x\approx 11.4840m$$

#### B --> C
'A' est sur la résistance

$\Delta t = 51.60ns$ entre impulsion 1 et reflection 1
$\implies 1.98\cdot10^8\cdot 51.60\cdot10^{-9}$
$$\Delta x\approx 10.2168m$$

### Résultats approximatif
$A + B +0C = 13.3452$
$A + 0B+ C = 11.4840$
$0A + B + C = 10.2168$

Avec *Gauss-Jordan*, il est possible de trouver a, b et c :

| A   | B   | C   | $\Delta x$ |
| --- | --- | --- | ---------- |
| 1   | 1   | 0   | 15.77      |
| 1   | 0   | 1   | 13.57      |
| 0   | 1   | 1   | 12.07      |

$A = 7.3062m$
$B = 6.0390m$
$C = 4.1778m$


## Fréquentielle
$$\hat{V}(z) = \hat{V}^+e^{-j\beta z} + \hat{V}^-e^{j\beta z}$$$$\hat{I}(z) = \dfrac{\hat{V}^+}{Z_c}e^{-j\beta z} - \dfrac{\hat{V}^-}{Z_c}e^{j\beta z}$$, où $\beta = \dfrac{\omega}{v}rads/m$


---
aaa
$$\lambda = \dfrac{v}{f} = v\cdot T$$

$v = 1.98\cdot10^8m/s$


#### A (isolé)
$f=6.6*10^6Hz$, alors
$$\lambda = \dfrac{1.98\cdot10^8}{6.6\cdot10^6}\approx 30.0000m$$
$$\mathscr{L}=\dfrac{\lambda}{4}\approx7.5m$$

#### B (isolé)
$f=8.08*10^6Hz$, alors
$$\lambda = \dfrac{1.98\cdot10^8}{8.08\cdot10^6}\approx 24.5040m$$$$\mathscr{L}=\dfrac{\lambda}{4}\approx6.126m$$

#### C (isolé)
$f=11.46*10^6Hz$, alors
$$\lambda = \dfrac{1.98\cdot10^8}{11.46\cdot10^6}\approx 17.255m$$$$\mathscr{L}=\dfrac{\lambda}{4}\approx4.319m$$

## Conclusion

| Cable | Temporel (m) | Fréquentiel (m) |
| ----- | ------------ | --------------- |
| A     | 7.3062       | 7.500           |
| B     | 6.0390       | 6.126           |
| C     | 4.1778       | 4.319           |
