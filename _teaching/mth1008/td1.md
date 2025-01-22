---
title: "TD1 : Matrices par blocs, indépendance linéaire et inversion de matrices"
permalink: /teaching/mth1008/td1
---

## Question de cours

Une famille \\(\\{v_1,...,v_p\\}\\) de vecteurs de \\(\mathbb{R}^n\\) est dite *liée* si un des vecteurs \\(v_i\\) (\\(i\in\\{1,...,p\\}\\)) s'exprime comme une combinaison linéaire des \\(p-1\\) autres vecteurs. Ceci se réécrit comme : il existe \\(i\in\\{1,...,p\\}\\) et des scalaires \\(\beta_1,...,\beta{i-1},\beta{i+1},...,\beta\in\mathbb{R}\\) tels que :

$$
    v_i=\beta_1v_1+...+\beta_{i-1}v_{i-1}+\beta_{i+1}v_{i+1}+...+\beta_pv_p=\sum_{\substack{j=1\\ j\neq i}}^p\beta_jv_j.
$$

Pourtant, la définition donnée par le cours dit qu'il doit exister des scalaires \\(\alpha_1,...,\alpha_p\in\mathbb{R}\\) **dont au moins un non nul**, tels que :

$$
    \alpha_1v_1+...+\alpha_pv_p=\sum_{j=1}^p\alpha_jv_j=0_n,
$$
où \\(0_n\\) désigne le vecteur de \\(\mathbb{R}^n\\) rempli de zéros.

Montrez que ces deux définitions sont bien équivalentes.

<details>
    <summary>Correction</summary>
    Le plus simple est de partir de la définition donnée dans le cours pour montrer qu'une relation de dépendance linéaire y est cachée. Supposons donc que l'on a une famille \\(\{v_1,...,v_p\}\\) de vecteurs de \\(\mathbb{R}^n\\) et des réels \\(\alpha_1,...,\alpha_p\\) tels que
    
    $$
        \alpha_1v_1+...+\alpha_pv_p=\sum_{j=1}^p\alpha_jv_j=0_n.
    $$

    Supposons qu'il existe un \\(\alpha_i\\) (où l'indice \\(i\\) est choisi dans \\(\{1,...,p\}\\)) tel que \\(\alpha_i\neq 0\\). On peut alors faire ressortir le terme \\(\alpha_iv_i\\) de notre somme : on a
    $$
        \alpha_iv_i+\left(\alpha_1v_1+...+\alpha_{i-1}v_{i-1}+\alpha_{i+1}v_{i+1}+...+\alpha_pv_p\right)=0_n
    $$
    *(On a simplement mis un terme en évidence dans la somme.)*
    
    On réarrange ceci en faisant passer la parenthèse de l'autre côté de l'égalité. Puisque \\(\alpha_i\neq 0\\), on peut ensuite diviser et on obtient :
    $$
        v_i=-\left(\frac{\alpha_1}{\alpha_i}v_1+...+\frac{\alpha_{i-1}}{\alpha_i}v_{i-1}+\frac{\alpha_{i+1}}{\alpha_i}v_{i+1}+...+\frac{\alpha_p}{\alpha_i}\right)=-\frac{1}{\alpha_i}\sum_{\substack{j=1\\ j\neq i}}\alpha_jv_j.
    $$
    Et ceci est une expression de \\(v_i\\) comme combinaison linéaire des \\(p-1\\) autres vecteurs, où on a fixé
    $$
        \beta_j=-\frac{\alpha_j}{\alpha_i}.
    $$
    Les 2 définitions sont bien équivalentes.
</details>

## Exercices

| Section                                        | Routine | Intermédiaire      | Approfondi |
| ---------------------------------------------- | ------- | ------------------ | ---------- |
| §1.4. L'équation matricielle \\(Ax=b\\)        |         |                    | 14         |
| §1.7. Indépendance linéaire                    | 2, 10   | 14, 18, 20, 22, 24 | 32         |
| §2.2. Inverse d'une matrice                    | 3, 6    | 13, 18, 20, 32     | 8          |
| §2.3. Caractérisation des matrices inversibles | 2, 4    | 14, 16, 23         | 26         |
| §2.4. Matrices par blocs                       | 8       | 12, 21, 25         |            |


*[Routine]: Exercices de base pour éveiller les premiers réflexes.
*[Intermédiaire]: Exercices de calcul ou réflexion constituant la matière principale de l'examen.
*[Approfondi]: Exercices allant plus loin que les calculs classiques. Ils ne sont pas toujours (mais souvent) les plus compliqués et vous prépareront aux questions d'examen nécessitant plus de réflexion personnelle.