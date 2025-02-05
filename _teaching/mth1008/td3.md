---
title: "TD3 : Propriétés des déterminants, espaces vectoriels (partie 1)"
permalink: /teaching/mth1008/td3
---

## Questions de cours

### Sous-espaces vectoriels de \\(\mathbb{R}^{n\times n}\\) (examen final, A2024)

L'espace des matrices carrées \\(n\times n\\) à coefficients réels est un espace vectoriel. Les ensembles suivants en sont-ils des sous-espaces vectoriels ?

a. L'ensemble des matrices inversibles

b. L'ensemble des matrices antisymétriques, i.e. telles que \\(A^\top=-A\\).

#### Solutionnaire

a. Vous devez immédiatement remarquer que cet ensemble n'est pas un sous-espace vectoriel, car il ne vérifie pas la toute première propriété : \\(0\\) n'est pas inversible ! Attention : ici, on est dans un espace vectoriel de matrices, vous devez donc comprendre le \\(0\\) comme la matrice nulle :

$$\begin{bmatrix}0 & \cdots & 0\\ \vdots & \ddots & \vdots\\ 0 & \cdots & 0\end{bmatrix}.$$

Évidemment, cette matrice n'est pas inversible.

b. Celle-ci est moins évidente, allons-y étape par étape.

- L'élément nul \\(0\\) est de nouveau la matrice nulle. Cette matrice est effectivement antsymétrique puisque

$$\begin{bmatrix}0 & \cdots & 0\\ \vdots & \ddots & \vdots\\ 0 & \cdots & 0\end{bmatrix}^\top=\begin{bmatrix}0 & \cdots & 0\\ \vdots & \ddots & \vdots\\ 0 & \cdots & 0\end{bmatrix}=-\begin{bmatrix}0 & \cdots & 0\\ \vdots & \ddots & \vdots\\ 0 & \cdots & 0\end{bmatrix}$$.

- Considérons \\(A\\) une matrice antisymétrique et \\(\alpha\in\mathbb{R}\\). Vérifions que la matrice \\(\alpha A\\) est bien antisymétrique. Pour cela, évitez d'écrire une matrice au long, vous allez vous perdre. Rappelez-vous simplement que quand on multiplie une matrice par un scalaire, on obtient : \\((\alpha A)^\top=\alpha A^\top\\) (cette fois, vous pouvez écrire une matrice pour vous en convaincre). Ici, on a donc :

$$(\alpha A)^\top=\alpha A^\top=\alpha(-A)=-(\alpha A).$$

Donc la matrice \\(\alpha A\\) est antisymétrique également.

- Considérons 2 matrices \\(A\\) et \\(B\\) antisymétriques, i.e. \\(A^\top=-A\\) et \\(B^\top=-B\\). Rappelez-vous la formule : si \\(A\\) et \\(B\\) sont de mêmes dimensions, on a \\((A+B)^\top=A^\top+B^\top\\). Ainsi :

$$(A+B)^\top=A^\top+B^\top=-A+(-B)=-(A+B).$$

Donc la matrice \\(A+B\\) est également antisymétrique.

Conclusion : les 3 propriétés sont vérifiées, l'ensemble des matrices carrées antisymétriques est donc un sous-espace vectoriel de \\(\mathbb{R}^{n\times n}\\).

### Prélude aux séries de Fourier

L'exercice §4.1-20 propose de montrer que l'ensemble \\(\mathcal{C}([a,b])\\) des fonctions continues sur un intervalle \\([a,b]\\) est un espace vectoriel (rappel : un *sous-espace vectoriel* est avant tout un espace vectoriel lui-même). Montrer que l'ensemble \\(\mathcal{C}_T([a,b])\\) des fonctions périodiques de période \\(T>0\\) est un sous-espace vectoriel de \\(\mathcal{C}([a,b])\\).

Rappel : une telle fonction est dite périodique de période \\(T\\) si pour tout \\(x\in[a,b-T]\\), on a \\(f(x+T)=f(x)\\).

#### Solutionnaire

Même démarche, mais ici on manipule des objets un peu différents : des fonctions.

- Nous sommes dans un espace de fonctions, l'élément nul est donc une fonction ! Il s'agit de la fonction que l'on notera \\(0 : [a,b]\to \mathbb{R}\\) qui vérifie : pour tout \\(x\in[a,b], 0(x)=0\\). Cette fonction est bien sûr périodique puisque dès lors que \\(x\in[a,b]\\), on a \\(0(x+T)=0=0(x)\\).
- Considérons \\(f\in\mathcal{C}_T([a,b])\\) et \\(\alpha\in\mathbb{R}\\). Montrons que la fonction \\(\alpha f\\) est également périodique de période \\(T\\). Pour tout \\(x\in[a,b-T]\\), on a \\((\alpha f)(x+T)=\alpha f(x+T)=\alpha f(x)\\). Donc \\(\alpha f\\) est également périodique, de période \\(T\\).
- Enfin, soient \\(f, g\in\mathcal{C}_T([a,b])\\). Montrons que la fonction \\(f+g\\) est également périodique de période \\(T\\). Pour \\(x\in[a,b-T]\\), on a \\((f+g)(x+T)=f(x+T)+g(x+T)=f(x)+g(x)=(f+g)(x)\\). Donc \\(f+g\\) est bien \\(T\\)-périodique.

## Exercices

| Section                                           | Routine | Intermédiaire  | Approfondi |
| ------------------------------------------------- | ------- | -------------- | ---------- |
| §3.1. Introduction aux déterminants               |         |                | 41         |
| §3.2. Propriétés des déterminants                 | 3, 4    | 8, 14, 24      | 31         |
| §4.1. Espaces vectoriels, sous-espaces vectoriels | 1, 3    | 8, 12, 18      | 32         |
| §4.2. Noyau, image et applications linéaires      | 18, 20  | 8, 16, 24      | 29         |
| §4.3. Familles libres et bases                    | 4, 24   | 10, 14, 20, 25 |            |

[Exercice récapitulatif proposé par Théo Denorme et Nathan Allaire.](/files/TN-extrait-recap-bases.pdf)

*[Routine]: Exercices de base pour éveiller les premiers réflexes.
*[Intermédiaire]: Exercices de calcul ou réflexion constituant la matière principale de l'examen.
*[Approfondi]: Exercices allant plus loin que les calculs classiques. Ils ne sont pas toujours (mais souvent) les plus compliqués et vous prépareront aux questions d'examen nécessitant plus de réflexion personnelle.