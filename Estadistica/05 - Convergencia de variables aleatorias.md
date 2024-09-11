# Convergencia de variables aleatorias

## Ley de los grandes números

Si $X_1,\dots,X_n$ son variables aleatorias independientes e idénticmente distribuidas, la media muestral

$$
\bar{X}_n=\frac{1}{n}\sum_{i=1}^nX_i
$$

converge en probabilidad a la esperanza de $X_i$: 

$$
\mu=\mathbb{E}(X_i)
$$

Esto significa que $\bar{X}_n$ está cerca de $\mu$ con probabilidad "alta" cuando $n$ es "grande".

## Teorema del Límite Central

Si $X_1,\dots,X_n$ son variables aleatorias independientes e idénticmente distribuidas, $\sqrt{n}(\bar{X}_n-\mu)$ converge en distribución a la distribución normal $N(0,\sigma^2)$.

De forma equivalente:

$$
\frac{\sqrt{n}(\bar{X}_n-\mu)}{\sigma}\sim N(0,1)
$$

cuando $n\rightarrow \infty$.

### Teorema del Límite Central con varianza muestral

Si $X_1,\dots,X_n$ son variables aleatorias independientes e idénticmente distribuidas:

$$
\frac{\sqrt{n}(\bar{X}_n-\mu)}{S_n}\sim N(0,1)
$$