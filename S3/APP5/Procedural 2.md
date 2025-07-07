$$V_1 = V_{in}*\cos(\omega t-\beta z)$$$$v = \dfrac{\omega}{\beta} = \sqrt{\dfrac{1}{LC}} = \dfrac{v_0}{\sqrt{\varepsilon_r}}$$$$Z_c = \sqrt{\frac{L}{C}}$$
$$V_z = \mathbb{R}(V_{0}\cdot e^{j(\omega t- \beta z)})$$$$\implies V(z, t) = \mathbb{R}(V_{0}\cdot e^{\omega t} \cdot e^{-j\beta z})$$$$\implies \hat{V}(z) = V_{0}\cdot e^{-j\beta z}$$
### Reflections
Le coefficient ($\Gamma_L$) de l'onde de réflection
- 1 = circuit ouvert
- -1 = circuit fermé
- 0 = aucune reflection
- 
$V_{reflect}(z, t) = \Gamma_L\cdot V_0\cos(\omega t+\beta z)$

## E1
### a.
![[Pasted image 20250707093152.png|400]]

### b.
?

### c.
?

### d. Circuit fermé (-1)
Le signal sera reflété de façon inverse au signal de base, suivant l'equation suivante: 
$V^-(z, t) = \Gamma_L\cdot V_0\cos(\omega t+\beta z)$
L'addition des deux signaux donnera alors un point d'entree stationnaire (milieu a droite), avec une onde ne semble pas se déplacer à travers le temps. Son amplitude passe entre 2 et 0.
![[Pasted image 20250707094215.png|400]]![[Pasted image 20250707094253.png|400]]
### e. Circuit ouvert (1)
![[Pasted image 20250707094800.png|400]]

![[Pasted image 20250707094912.png|400]]

### f.
$$I(z,t) = \dfrac{V_0\cos(\omega t - \beta z)}{Z_c} - \dfrac{V_0\cos(\omega t + \beta z)}{Z_c}$$$$\implies I(z,t) = \dfrac{V^+}{Z_c}-\dfrac{V^-}{Z_c}$$

$$cos(a+b)=cos(a)cos(b)-sin(a)sin(b)$$$$\implies cos(a)-cos(b) = -2\cdot sin(\dfrac{a+b}{2})\cdot sin(\dfrac{a-b}{2})$$


$$I(z,t) = \dfrac{V_0(cos(\omega t -\beta z)- cos(\omega t +\beta z)}{Z_c}$$$$\implies \dfrac{-2V_0}{Z_c}sin(\dfrac{\omega t - \beta z + \omega t +\beta z}{2})$$$$\implies \dfrac{-2V_0}{Z_c}sin(\omega t)\cdot sin(-\beta z)$$$$\implies I(z,t) = \mathbb{I}\Big(\dfrac{2V_0}{Z_L} \cdot sin(-\beta z)\Big)\cdot e^{j\omega t}$$

## E2
### a. Coefficient de reflection à la charge
$$\hat{\Gamma}_L(\mathscr{L}) = \dfrac{\hat{Z}_L-Z_c}{\hat{Z}_L+Z_c}$$

### b. Coefficient de reflection ramené
Formule générale (z = point/distance):
$$\hat{\Gamma}_L(z) = \hat{\Gamma}_L\cdot e^{j\cdot2\beta(z-\mathscr{L})}$$
Lorsque $z =0$ :
$$\hat{\Gamma}_L(0) = \hat{\Gamma}_L\cdot e^{-j\cdot2\beta\
\mathscr{L}}$$

### c. Impédance ramené
$$\hat{Z}_{in}=Z_c\dfrac{1+\hat{\Gamma}_L(0)}{1-\hat{\Gamma}_L(0)}$$

### d.
Si $Z_{in} = Z_c$ alors avec la formule vu [[S3/APP5/Procedural 2#a. Coefficient de reflection à la charge|ici]], on peut d/terminer que $\Gamma_L = 0$.

## E3

Si $\beta = \dfrac{2\pi}{\lambda}$, et que $\mathscr{L} = \dfrac{\lambda}{4}$alors:
$$v = \dfrac{\omega}{\beta} = \dfrac{2\pi f}{\beta}$$$$v = \dfrac{\lambda}{t} = \lambda\cdot f$$
$$\hat{Z}_{in}=Z_c\dfrac{1+\hat{\Gamma}_L}{1-\hat{\Gamma}_L}\cdot e^{-j2\beta\mathscr{L}}$$Puisque $e^{-j2\beta\mathscr{L}} = e^{-j\cdot2\cdot\frac{2\pi}{\lambda}\frac{\lambda}{4}} = e^{-j\pi} = -1$, et que $\hat{\Gamma}_L = \dfrac{\hat{Z}_L-Z_c}{\hat{Z}_L+Z_c}$, alors : $$\hat{Z}_{in}=-1\cdot Z_c\dfrac{1-\frac{\hat{Z}_L-Z_c}{\hat{Z}_L+Z_c}}{1+\frac{\hat{Z}_L-Z_c}{\hat{Z}_L+Z_c}}$$$$\implies \hat{Z}_{in} = Z_c\dfrac{\hat{Z}_c+Z_c-\hat{Z}_c+Z_c}{\hat{Z}_L+Z_c+\hat{Z}_L-Z_L} = \dfrac{2Z_c}{2\hat{Z}_L}$$$$\implies Z_{in} = \dfrac{Z_c^2}{\hat{Z}_L}$$
## E4

Soit : 
- $f=20MHz$,
- $V_s=50\angle 0\degree$, 
- $v = 2\cdot10^8m/s$, 
- $\mathscr{L}=52m$, 
- $Z_c=50\Omega$, 
- $Z_s = 20-j30\Omega$, 
- $Z_L = 200-j500\Omega$


### a. 
$$v= \dfrac{\lambda}{t} = \lambda f$$$$\implies \lambda = \dfrac{v}{f} = \dfrac{2\cdot10^8}{5\cdot10^6} = 40m$$

### b. Coefficient de reflection de tension a la charge
[[S3/APP5/Procedural 2#a. Coefficient de reflection à la charge|Formule de base]]
$$\implies \dfrac{150-j500}{250-j500} = \dfrac{3-10j}{5-10j}$$$$\dfrac{(3-10j)(5+10j)}{\sqrt{5^2+10^2}}\approx 0.9338\cdot e^{-j\cdot0.172} = \hat{\Gamma}_L$$
### c. Coefficient de reflection de tension a la charge, ramené a la source
[[S3/APP5/Procedural 2#b. Coefficient de reflection ramené|Formule de base (voir générale)]]
$$0.9338\cdot e^{-j\cdot0.172}\cdot e^{-jw\frac{2\pi}{\lambda}1.3\lambda}$$$$\hat{\Gamma}_{in}=0.9338\cdot e^{-j\cdot2.34}$$
### d. Impédance de la charge ramenée à la source
[[S3/APP5/Procedural 2#c. Impédance ramené|Formule de base]]
$$\hat{Z}_{in} = Z_c\dfrac{1+\Gamma_{in}}{1-\Gamma_{in}}$$
$$\implies50\cdot\dfrac{1+0.9338\cdot e^{-j\cdot2.34}}{1-0.9338\cdot e^{-j\cdot2.34}}$$

### e. Tension en fonction du temps a la source
$$\hat{V}_{in} = V_s\cdot\dfrac{\hat{Z}_{in}}{\hat{Z}_{in}+Z_s}$$ Cest un diviseur de tension!
Soit :
- $\hat{V}_s = 50\cdot e^{-j\beta z}$
- $z = 0$
Donc, 
$$\hat{V}_{in} = 50\cdot\dfrac{\hat{Z}_{in}}{\hat{Z}_{in}+Z_s}$$

### f. Puissance 

Puisqu'on travaille en RMS ($\frac{1}{\sqrt{2}}$), alors il est possible de simplement faire $\frac{1}{\sqrt{2}}\cdot\frac{1}{\sqrt{2}} =\cdot \dfrac{1}{2}$ lorsqu'on travaille avec les puissances
$P=V_{RMS}I_{RMS} = \dfrac{VI}{2} = \dfrac{V^2}{2R} = \dfrac{1}{2}RI^2$
$$P=\dfrac{|V|^2}{2\cdot\mathbb{R}(Z_{in})}$$

### g. Taux d'onde stationnaire
Rapport d'onde stationnaire (ROS)
Taux d'onde stationnaire (TOS)

$$ROS = \dfrac{V_{max}}{V_{min}} = \dfrac{V_i+V_r}{V_i-V_r}$$
$$TOS = 100\cdot\dfrac{ROS-1}{ROS+1}$$
