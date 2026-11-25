#estatistica 

Distribuição contínua **simétrica** ao redor da média $\large \mu$, onde valores próximos da média ocorrem mais do que valores afastados.
A soma da área embaixo da curva é sempre 1.
Também conhecida como distribuição normal ou de sino.

![[gaussian_distribution.png|700]]

A [[Função Densidade de Probabilidade]] (PDF) da distribuição gaussiana é:
$$
\LARGE f(x) = \frac{1}{\sigma \sqrt{2\pi}}e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$
$$
\begin{aligned}
& x = \text{valor da variável} \\
& \mu = \text{média da distriuição} \\
& \sigma = \text{desvio padrão}
\end{aligned}
$$

Para calcular a probabilidade e um valor e estar entre $a$ e $b$, usa-se a integral definida de $f(x)$:
$$
\large P(a \le X \le b) = \int^b_a f(x) \; dx
$$

## Regra 68-95-99.7
- Aproximadamente $68\%$ dos dados caem no intervalo de 1 desvio padrão.
- $95\%$ no intervalo de 2 desvios padrão
- $99.7\%$ no intervalo de 3 desvios padrão

## Distribuição Normal Padrão
Também chamada de Z-Distribution, possui média $\mu = 0$ e desvio padrão $\sigma = 1$
Sua [[Função Densidade de Probabilidade|PDF]] é:
$$
\LARGE f(z) = \frac{1}{\sqrt{2\pi}}e^{\frac{-z^2}{2}}
$$
Onde $z$ é o valor normalizado:
$$
\large Z = \frac{x - \mu}{\sigma}
$$

Uma maneira muito mais fácil de calcular a área embaixo da curva é usar uma [Z-Table](https://www.ztable.net/). É possível encontrar o valor da área de $-\infty$ até $z$.

- - -

## Exemplo — 1
> Uma fábrica produz garrafas cuja quantidade de líquido segue uma distribuição normal com média $\mu = 500$ ml e desvio padrão $\sigma = 10$ ml.

> $a)$ Qual é a probabilidade de uma garrafa conter menos de 490 ml?
> $b)$ Qual é a probabilidade de conter entre 490 e 510 ml?
> $c)$ Qual é a probabilidade de conter mais de 520 ml?

$$
\begin{aligned}
& a) \quad Z = \frac{490 - 500}{10} = -1 \\
& \text{Seguindo a Z-table:} \approx15.9\%
\end{aligned}
$$

$$
\begin{aligned}
& b) \quad Z_1 = \frac{490 - 500}{10} = -1 \\
& \qquad Z_2 = \frac{510 - 500}{10} = 1 \\
& Z_2 - Z_1 = 84.13 - 15.86 = \; \approx68.3\%
\end{aligned}
$$

$$
\begin{aligned}
& a) \quad Z = \frac{520 - 500}{10} = 2 \\
& 1 - 0.9772 = \; \approx2.3\%
\end{aligned}
$$