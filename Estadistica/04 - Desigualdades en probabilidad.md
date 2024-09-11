# Desigualdades en probabilidad

## Desigualdad de Markov

Sea $X$ una variable aleatoria **no negativa** y supongamos que $\mathbb{E}(X)$ existe. Para cualquier $t>0$:

$$
\mathbb{P}(X>t)\leq \frac{\mathbb{E}(X)}{t}
$$

## Desigualdad de Chebyshev

Sean $\mu=\mathbb{E}(X)$ y $\sigma^2=\mathbb{V}(X)$. Entonces

$$
\mathbb{P}(|X-\mu|\geq t)\leq \frac{\sigma^2}{t^2}
$$

$$
\mathbb{P}(|Z|\geq k)\leq \frac{1}{k^2}
$$

donde $Z=(X-\mu)/\sigma$.

### Tabla de cotas probabilísticas

Si $X$ es una variable aleatoria **no negativa**, entonces los porcentajes de la siguiente tabla representan la probabilidad de que $X$ esté dentro (o fuera) del intervalo $[\mu - k\sigma, \mu + k\sigma]$.

| k | Mín. % dentro de $k$ desviaciones estándar alrededor de la media | Máx. % fuera de $k$ desviaciones estándar alrededor de la media |
| --- | --- | --- |
| 1 | 0% | 100% |
| $\sqrt{2}$ | 50% | 50% |
| 2 | 75% | 25% |
| 3 | 88.8889% | 11.1111% |
| 4 | 93.75% | 6.25% |
| 5 | 96% | 4% |
| 6 | 97.2222% | 2.7778% |
| 7 | 97.9592% | 2.0408% |
| 8 | 98.4375% | 1.5625% |
| 9 | 98.7654% | 1.2346% |
| 10 | 99% | 1% |

## Desigualdad de Hoeffding (para var. Bernoulli)

Sean $X_1,\dots,X_n\sim\text{Bernoulli}(p)$. Entonces, para cualquier $\epsilon>0$,

$$
\mathbb{P}(|\bar{X}-p|>\epsilon)\leq 2e^{-2n\epsilon^2}
$$

donde $\bar{X}=\frac{1}{n}\sum_{i=1}^nX_i$.

## Desigualdad de Mill

Sea $Z\sim N(0,1)$, entonces

$$
\mathbb{P}(|Z|>t)\leq \sqrt{\frac{2}{\pi}}\cdot \frac{e^{-t^2/2}}{t}
$$