---
title: "TD5 : Applications linéaires"
permalink: /teaching/mth1008/td5
---

## Questions de cours

### Équivalence injectivité \\(\Leftrightarrow\\) surjectivité pour les matrices carrées

Soit \\(T\\) un endomorphisme de \\(\mathbb{R}^n\\), c'est-à-dire une application linéaire de \\(\mathbb{R}^n\\) dans \\(\mathbb{R}^n\\). Montrer que \\(T\\) est surjective si et seulement si (\\(\Leftrightarrow\\)) \\(T\\) est injective. Autrement dit, pour une matrice carrée, l'injectivité et la surjectivité de l'application linéaire associée sont 2 notions équivalentes.

### L'isomorphisme sauveteur

La semaine passée, nous avons vu que les opérations sur les espaces de polynômes semblaient plus faciles lorsque l'on regarde le polynôme

$$p(t)=a_nt^n+...+a_1t+a_0\in\mathbb{P}_n$$

comme le vecteur de \\(\mathbb{R}^{n+1}\\) regroupant ses composantes, i.e. :

$$p(t)\to \begin{bmatrix}a_0\\ a_1\\ \vdots\\ a_n\end{bmatrix}\in\mathbb{R}^{n+1}.$$

Cette astuce est justifiée par l'existence d'une correspondance naturelle entre \\(P_n\\) et \\(R^{n+1}\\). Cette correspondance s'appelle un *isomorphisme*.

Considérons l'application \\(T : \mathbb{P}_n\to\mathbb{R}^{n+1}\\) définie pour tout polynôme \\(p(t)=a_nt^n+...+a_1t+a_0\\) par :

$$T(p)=\begin{bmatrix}a_0\\ a_1\\ \vdots\\ a_n\end{bmatrix}.$$

Montrez que cette application est linéaire et bijective. La propriété de bijectivité fait de \\(T\\) un *isomorphisme* entre \\(\mathbb{P}_n\\) et \\(\mathbb{R}^n\\).

## Exercices

| Section                                       | Routine | Intermédiaire | Approfondi |
| --------------------------------------------- | ------- | ------------- | ---------- |
| §1.8. Introduction aux applications linéaires |         |               |            |
| §1.9. Matrice d'une application linéaire      |         |               |            |

*[Routine]: Exercices de base pour éveiller les premiers réflexes.
*[Intermédiaire]: Exercices de calcul ou réflexion constituant la matière principale de l'examen.
*[Approfondi]: Exercices allant plus loin que les calculs classiques. Ils ne sont pas toujours (mais souvent) les plus compliqués et vous prépareront aux questions d'examen nécessitant plus de réflexion personnelle.