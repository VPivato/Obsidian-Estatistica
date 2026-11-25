#estatistica

## Amplitude
Medida mais simples e fácil de calcular, é muito sensível a valores extremos (outliers). Corresponde simplesmente à diferença entre o maior e menor valor.
$$
Amplitude = X_{max} - X_{min}
$$

## Amplitude Interquartil — IQR
Indica a variação ou espalhamento dos 50% centrais de um conjunto de dados. Métrica mais robusta contra outliers. Usado em Boxplots.
$$
IQR = Q_3 - Q_1
$$
A mediana do conjunto representa $Q_2$. Calcular a mediana da metade inferior de $Q_2$ nos dá $Q_1$, calcular a mediana da metade superior de $Q_2$ nos dá $Q_3$.

## Desvio Padrão
Medida que indica o quanto os valores de um conjunto tendem a se distanciar da média aritmética. A fórmula difere entre o desvio padrão amostral e populacional

Amostral:
$$
\large s = \sqrt \frac{\sum{(x - \bar{x})^2}}{n - 1}
$$
Populacional:
$$
\large \sigma = \sqrt \frac{\sum{(x - \mu)^2}}{N}
$$