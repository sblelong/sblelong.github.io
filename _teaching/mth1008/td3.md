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

$$\begin{bmatrix}0 & \cdot & 0\\ \vdots & \ddots & \vdots\\ 0 & 0 & 0\end{bmatrix}.$$

### Prélude aux séries de Fourier

L'exercice §4.1-20 propose de montrer que l'ensemble \\(\mathcal{C}([a,b])\\) des fonctions continues sur un intervalle \\([a,b]\\) est un espace vectoriel (rappel : un *sous-espace vectoriel* est avant tout un espace vectoriel lui-même). Montrer que l'ensemble \\(\mathcal{C}_T([a,b])\\) des fonctions périodiques de période \\(T>0\\) est un sous-espace vectoriel de \\(\mathcal{C}([a,b])\\).

Rappel : une fonction est dite périodique de période \\(T\\) si pour tout \\(x\in[a,b]\\), on a \\(f(x+T)=f(x)\\).

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