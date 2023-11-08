---
title: "Unmodeled Interaction in Binary Dependent Variable Model"
collection: publications
excerpt: "Under social sciences contexts, factors exhibit various forms of correlation, and it's not easy for reseachers to capture the correct relationships. Incorrect model specification can bring unmodeled interactions which further causes bias in estimation and predictions. In this project, We focused on the logistic regression and tried to utilize Neural Networks as a supplementary tool to help to identify the model specification. "
---

\* This Project is with _Professor Moy_, a research faculty at NYU Center for Data Science and the Department of Politics. 

**Simple Example** \
Here is a straightforward case for bias brought by model misspecification. $Z_1$ and $Z_2$ are correlated with each other, and are drawn from a multivariate normal distribution with $\rho$ = 0.5; $Z_2$ is categorized to a binary variable. $X \sim  N(Z_1+Z_2,1)$.

**True model** - $y=\beta_{1}X+\beta_{2}Z_1+\beta_{3}X*Z_1+\beta_{4}Z_2$ 

**Incorrect model 1 (no interaction)** -
$y=\beta_{1}X+\beta_{2}Z_1+\beta_{3}Z_2$ 

**Incorrect model 2 (wrong interaction)** -
$y=\beta_{1}X+\beta_{2}Z_1+\beta_{3}X*Z_2+\beta_{4}Z_2$ 

**Incorrect model 3 (full interaction)** -
$y=\beta_{1}X+\beta_{2}Z_1+\beta_{3}Z_3+\beta_{4}X*Z_1+\beta_{5}X*Z_2+\beta_{6}Z_1*Z_2$

 