---
title: "TD1 : Matrices par blocs, indépendance linéaire et inversion de matrices"
permalink: /teaching/mth1008/td1
---

## Question de cours

Une famille \\(\\{\mathbf{v}_1,...,\mathbf{v}_p\\}\\) de vecteurs de \\(\mathbb{R}^n\\) est dite *liée* si un des vecteurs \\(\mathbf{v}_i\\) (\\(i\in\\{1,...,p\\}\\)) s'exprime comme une combinaison linéaire des \\(p-1\\) autres vecteurs. Ceci se réécrit comme : il existe \\(i\in\\{1,...,p\\}\\) et des scalaires \\(\alpha_1,...,\alpha_{i-1},\alpha_{i+1},...,\alpha_p\in\mathbb{R}\\) tels que :

$$
    \mathbf{v}_i=\alpha_1\mathbf{v}_1+...+\alpha_{i-1}\mathbf{v}_{i-1}+\alpha_{i+1}\mathbf{v}_{i+1}+...+\alpha_p\mathbf{v}_p=\sum_{\substack{j=1\\ j\neq i}}^p\alpha_j\mathbf{v}_j.
$$

Pourtant, la définition donnée par le cours dit qu'il doit exister des scalaires \\(\alpha_1,...,\alpha_p\in\mathbb{R}\\) **dont au moins un non nul**, tels que :

$$
    \alpha_1v_1+...+\alpha_pv_p=\sum_{j=1}^p\alpha_jv_j=\mathbf{0}.
$$

Montrez que ces deux définitions sont bien les mêmes.

## Exercices

| Section                                        | Routine | Intermédiaire | Approfondi |
| ---------------------------------------------- | ------- | ------------- | ---------- |
| §1.4. L'équation matricielle \\(Ax=b\\)        |         |               | 14         |
| §1.7. Indépendance linéaire                    |         |               |            |
| §2.2. Inversion de matrices                    |         |               |            |
| §2.3. Caractérisation des matrices inversibles |         |               |            |
| §2.4. Matrices par blocs                       |         |               |            |


*[Routine]: Exercices de base pour éveiller les premiers réflexes.
*[Intermédiaire]: Exercices de calcul ou réflexion constituant la matière principale de l'examen.
*[Approfondi]: Exercices allant plus loin que les calculs classiques. Ils ne sont pas toujours (mais souvent) les plus compliqués et vous prépareront aux questions d'examen nécessitant plus de réflexion personnelle.