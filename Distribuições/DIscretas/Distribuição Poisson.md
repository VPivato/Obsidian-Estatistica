#estatistica 

Calcula a chance de um certo número de eventos acontecer dentro de um intervalo fixo (tempo, espaço ou outra dimensão), assumindo que são independentes.
Caracterizada por um único parâmetro $\lambda$, que representa a ocorrência média de determinado evento em um intervalo de tempo.

Sua [[Função Massa de Probabilidade]] (PMF) é:
$$
\large P(X = k) = \frac{e^{-\lambda} \lambda^k}{k!}
$$
$$
\begin{aligned}
& e = 2.71828... \\
& \lambda = \text{taxa média de ocorrência dos eventos} \\
& k = \text{número de eventos que ocorem}
\end{aligned}
$$

Pontos chave:
- Eventos ocorrem de forma independente entre si.
- Quantidade de eventos pode assumir qualquer número inteiro não negativo.
- $\lambda$ é constante durante o intervalo

> [!TIP] Dica para $\lambda$
> O valor de lambda escala com o intervalo.
> Se $\large \lambda = 4/h$, um exercício que peça a taxa de ocorrência de eventos em um período de **meia hora** teria $\large \lambda = 2$.
> Isso funciona pois assumimos que a taxa é constante e cada evento independente.
## Exemplo — 1
>Uma padaria recebe, em média, 4 clientes por hora durante a manhã.
>	a) Qual é a probabilidade de chegarem exatamente 2 clientes na próxima hora?
>	b) Qual é a probabilidade de nenhum cliente chegar na próxima hora?

$$
\begin{aligned}
& \large \text{a)} \quad \frac{e^{-4} 4^2}{2} = 8e^{-4} = 0.1465... = \; \approx14.6\% \\
& \large \text{b)} \quad \frac{e^{-4}4^{0}}{1} = e^{-4} = 0.0183... = \; \approx1.8\%
\end{aligned}
$$

## Poisson como aproximação Binomial
Na [[Distribuição Binomial]], caso o número de tentativas seja muito grande e a probabilidade de sucesso seja muito baixa, é possível fazer uma aproximação usando a distribuição Poisson, onde:
$$
\large \lambda = n \times p
$$
Por exemplo:
> Uma fábrica produz 10.000 peças com uma taxa de defeito de 0.01%, qual a chance de 5 ou mais peças saírem defeituosas? ($\lambda = 10000 \times 0.0001 = 1$)

|  $k$   |       $P(X = k)$        | Resultado |
| :----: | :---------------------: | :-------: |
|  $0$   | $\frac{e^{-1} 1^0}{0!}$ | $36.79\%$ |
|  $1$   | $\frac{e^{-1} 1^1}{1!}$ | $36.79\%$ |
|  $2$   | $\frac{e^{-1} 1^2}{2!}$ | $18.40\%$ |
|  $3$   | $\frac{e^{-1} 1^3}{3!}$ | $6.13\%$  |
|  $4$   | $\frac{e^{-1} 1^4}{4!}$ | $1.53\%$  |
| $\sum$ |            -            | $99.64\%$ |
Portanto, a chance de 5 ou mais peças defeituosas é de $\approx0.36\%$. Ao usar a distribuição binomial, seria necessário fazer cálculos inviáveis manualmente, por exemplo:
$$
\large P(X = 4) = \binom{10000}{4}0.0001^4(0.9999)^{9996}
$$

## Materiais de Referência
- UFMG: https://www.est.ufmg.br/~monitoria/Material/ApostilaR/DistribuicoesProbabilidade.html
- GeeksForGeeks: https://www.geeksforgeeks.org/maths/poisson-distribution/