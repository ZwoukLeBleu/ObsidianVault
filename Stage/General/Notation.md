Pour representer un etat $\ket{\psi}$ a n-qubits, au lieu de l'ecrire comme etant 
$$\ket{\psi}= \alpha\ket{00..0} + \beta\ket{00..1}+\dots \pi\ket{11..1}$$ La sommation sera plutot utiliser, pour alleger la notation :
$$j= \sum_{q=0}^2 2^q\cdot b_q \qquad \qquad \qquad \ket{\psi}=\sum_{j=0}^7 \alpha_j\cdot\ket{j}$$

Les etats de bases a n-qubits peuvent etre construit à l'aide du produit tensoriel de n etats a un qubit:
$$\ket{b_{n-1}}\otimes\dots\otimes\ket{b_1}\otimes\ket{b_0}=\ket{b_{n-1}\dots b_1 b_0}= \bigotimes^{n-1}_{q=0}  \ket{b_q}$$
, qui devient plus succinctement
$$\ket{j}=\bigotimes_{q=0}^{2^n-1}\ket{b_q} \qquad \qquad \qquad j=\sum_{q=0}^{n-1} 2^q\cdot b_q$$
Et ensuite:
$$\implies \ket{\psi}=\sum_{j=0}^{2^n-1} \alpha_j\cdot\ket{j} \qquad \qquad \qquad \sum_{j=0}^{2^n-1} |\alpha_j|^2=1$$
