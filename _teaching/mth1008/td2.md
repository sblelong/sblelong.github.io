---
title: "TD2 : Noyau, rang, factorisation \\(LU\\) et déterminants"
permalink: /teaching/mth1008/td2
---

## Question de cours (exercice §1.5-26)

Soient \\(A\\) une matrice de taille \\(m\times n\\) à coefficients réels et \\(b\in\mathbb{R}^m\\). Supposons que le système linéaire \\(Ax=b\\) soit compatible. Montrer que la solution à ce système est unique si et seulement si (\\(\Longleftrightarrow\\)) \\(\mathrm{Ker}(A)=\\{0\\}\\).

### Correction

Un point de logique : supposons que le système soit compatible et notons
- \\(P\\) : la solution est unique
- \\(Q\\) : \\(\mathrm{Ker}(A)=\\{0\\}\\).

On vous demande ici de démontrer que \\(P\Longleftrightarrow Q\\). Ceci se fait en démontrant les 2 implications \\(P\implies Q\\) et \\(Q\implies P\\).

#### \\(P\implies Q\\)

Ce sens peut se démontrer par contraposée : on va en fait montrer que \\(\mathrm{Ker}(A)\neq\\{0\\}\implies\\) la solution n'est pas unique. Vous devriez l'avoir compris de votre cours : on peut ajouter des vecteurs du noyau à une solution particulière pour obtenir une autre solution. Rigoureusement, ceci s'écrit : soit \\(x\\) une solution du SÉL et soit \\(y\in\mathrm{Ker}(A)\\). On va supposer que \\(y\neq 0\\), c'est possible puisque que \\(\mathrm{Ker}(A)\neq\\{0\\}\\). On a alors :

$$A(x+y)=Ax+Ay=b+0=b$$

par la distributivité de la multiplication matrice-vecteur, \\(Ax=b\\) (puisque \\(x\\) est solution) et \\(y\in\mathrm{Ker}(A)\\). Donc le vecteur \\(x+y\\) est aussi une solution du SÉL, mais on est certain que \\(x+y\neq x\\) puisque \\(y\neq 0\\). Il existe donc au moins 2 solutions distinctes au SÉL dès que \\(\mathrm{Ker}(A)\neq\\{0\\}\\). On a donc montré que \\(\neq Q\implies\neq P\\), i.e. \\(P\implies Q\\).

#### \\(Q\implies P\\)

On veut ici montrer que si \\(\mathrm{Ker}(A)=\\{0\\}\\), alors la solution est unique. Pour ce faire, supposons que \\(\mathrm{Ker}(A)=\\{0\\}\\), et notons \\(x\in\mathbb{R}^n\\) une solution du SÉL.

Le secret de la preuve réutilise une astuce employée dans le sens \\(P\implies Q\\) : n'importe quel vecteur \\(y\neq x\\) peut s'écrire comme \\(x +\\) "un certain déplacement non-nul dans \\(\mathbb{R}^n\\)". Notons ce déplacement \\(z\in\mathbb{R}^n\setminus\\{0\\}\\), on a alors une écriture de forme \\(y=x+z\\) pour tout vecteur \\(y\neq x\\). Autrement dit, quand on calcule \\(Ay\\) pour tout \\(y\neq x\\), on a :

$$Ay=A(x+z)=Ax+Az=b+Az$$

par la distributivité de la multiplication matrice-vecteur, et parce que \\(Ax=b\\) (\\(x\\) est solution). Donc pour que \\(Ay=b\\) également, il faudrait que... \\(Az=0\\) ! Voyez-vous l'utilité du noyau ici ?

On a supposé que \\(z\neq 0\\), mais puisque \\(\mathrm{Ker}(A)=\\{0\\}\\), le seul moyen d'avoir \\(Az=0\\) serait que \\(z\in\mathrm{Ker}(A)\\), donc... \\(z=0\\) ! On a 2 hypothèses contraires (\\(z=0\\) et \\(z\neq 0\\)) donc ce \\(z\\) ne peut exister : la seule solution au système est \\(x\\).

## Exercices

À cause du mini-projet 1, seuls les exercices indiqués en *italique* seront traités pendant le TD. Les autres feront l'objet d'un corrigé écrit.

| Section                                             | Routine                | Intermédiaire | Approfondi |
| --------------------------------------------------- | ---------------------- | ------------- | ---------- |
| §1.5. Ensembles des solutions de systèmes linéaires | 5, *8*, *12*           | 14, 38        |            |
| §4.6. Rang                                          |                        | *19*, 25      | 30         |
| §2.5. Factorisations matricielles                   | *4*, *14*              | 21            | 24         |
| §3.1. Introduction aux déterminants                 | *Cours : exemple 5*, 4 | 24, 26        | 31         |


*[Routine]: Exercices de base pour éveiller les premiers réflexes.
*[Intermédiaire]: Exercices de calcul ou réflexion constituant la matière principale de l'examen.
*[Approfondi]: Exercices allant plus loin que les calculs classiques. Ils ne sont pas toujours (mais souvent) les plus compliqués et vous prépareront aux questions d'examen nécessitant plus de réflexion personnelle.

## Capsules de correction

- [Calcul rapide du noyau d'une matrice](https://youtu.be/dPulm6OioXY)
- Factorisation \\(LU\\)
  - [Résolution d'un système](https://youtu.be/kNg1zhz98i4)
  - [Calcul d'une factorisation](https://youtu.be/w8zb5liSURU)