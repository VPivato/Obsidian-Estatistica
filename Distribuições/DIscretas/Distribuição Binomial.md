Cálculo da probabilidade de obter determinado número de sucessos ao repetir um experimento várias vezes.
Cada experimento é independente e pode assumir dois resultados: sucesso ou falha.

Definida pela fórmula:
$$
\large P(X = k) = \binom{n}{k}p^k(1-p)^{n-k}
$$
$$
\begin{aligned}
& n = \text{número de tentativas} \\
& p = \text{probabilidade de sucesso} \\
& k = \{0,1,2...n\}\ \; \text{número de sucessos}
\end{aligned}
$$

Onde $\binom{n}{k}$ é o coeficiente binomial (combinação):
$$
\large \binom{n}{k} = \frac{n!}{k!(n-k)!}
$$

## Exemplo — 1
>Ao lançar um dado não viciado 3 vezes, crie uma distribuição de probabilidade teórica para a quantidade de números **6** obtidos.

$n = 3$, e $p = \frac{1}{6}$, pois são 3 tentativas distintas, e a chance de cair o lado 6 é de $\frac{1}{6}$. Portanto a fórmula se torna:
$$
\large P(X = k) = \binom{3}{k}\frac{1}{6}^k(\frac{5}{6})^{3-k}
$$
Em relação ao número de sucessos, pode-se obter $\{0,1,2,3\}$ dados 6 em 3 tentativas.

| $k$ |                   $P(X = k)$                   |     Resultado     |
| :-: | :--------------------------------------------: | :---------------: |
|  0  | $\binom{3}{0}(\frac{1}{6})^0(\frac{5}{6})^{3}$ | $\frac{125}{216}$ |
|  1  | $\binom{3}{1}(\frac{1}{6})^1(\frac{5}{6})^{2}$ | $\frac{75}{216}$  |
|  2  | $\binom{3}{2}(\frac{1}{6})^2(\frac{5}{6})^{1}$ | $\frac{15}{216}$  |
|  3  | $\binom{3}{3}(\frac{1}{6})^3(\frac{5}{6})^{0}$ |  $\frac{1}{216}$  |

Representação gráfica da probabilidade de obter K dados de lado 6 ao lançá-lo 3 vezes consecutivas:

![[binomial_distribution_example_1.svg|700]]
- - -
## Materiais de Referência
- UFMG: https://www.est.ufmg.br/~monitoria/Material/ApostilaR/DistribuicoesProbabilidade.html