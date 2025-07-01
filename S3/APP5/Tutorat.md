$sin(\omega t+kz)$, ou kz=déplacement

## Prototype 1
1MHz
Cable [[Coaxial]]

## Prototype 2
10MHz
Connecteur RG58u
Impedence des cartes de $50 \Omega$
Au minimum, l'amplitude doit depasser +/- 0.5V durant $\dfrac {1}{4}$ de periode

## Résolution de probleme
On ne peut pas acceder au cables, ni le connecteur en ***T*** (Ne pas toucher la bobine). On peut uniquemnet acceder au port A, B et C.

On recherche la longeur des cables?
On recherche:
1. Un [[Mode de transfers]] en Half-Dupex (*simple*)
2. Un mode Full-Duplex en remplaçant le ***T*** par un circuit passif (Seulement des résistances, aucune réflexion dans le réseau, *plus complexe*)
3. Si le réseau passif est possible, est ce qu'une horloge de 1GHz est possible, avec des centaines de connections en ***T***?

Signal qui se propage: 
$$v(t,z)=Acos(\omega t \pm kz)=\mathbb{R}(A\cdot e^{j(\omega t \pm kz)}) $$
$$v(z)=A\cdot e^{\pm j \cdot kz}\cdot e^{j\cdot \omega t} = phaseur$$

#### Reflections
- Lorsqu'on branche un cable en configuration T, est-ce que sont impédance reste la même dans les deux fils sortant, que le singulier fil entrant? *non, ils se font couper!*
- Une analyse temporelle risque d'etre peut fructueuse, les générateurs et oscilloscopes risquent d'arrondir trop fortement les valeurs lu. De ce, une analyse *fréquentielle* serait plus approprié
- 
### Reformulation 
Analyser un réseau pour le corriger, trouver les caractéristiques des fils (Analyse temporelle et fréquentielle), puis ensuite proposer des solutions 
