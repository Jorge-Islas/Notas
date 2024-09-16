# Fundamentos de Machine Learning

## Términos

- **Training data**: datos utilizados para ajustar los modelos

- **Testing data**: datos no utilizados para entrenar el modelo que son usados para probar el desempeño de este con nuevas observaciones / datos.

- **Sesgo / Bias**: La incapacidad de un modelo de ML para captar y representar la relación verdadera entre los datos.

- **Varianza (ML)**: Se refiere a qué tanto cambiarían las predicciones si el modelo se ajustara a un conjunto de entrenamiento distinto.

- **Sobreajuste / overfitting**: Cuando un modelo se ajusta "muy bien" al conjunto de entrenamiento, pero falla al predecir el cunjunto de prueba.

## Cosas por cuidar

- La muestra debe reflejar lo mejor posible a la población de estudio, puesto que, en caso contrario, esto puede causar un sesgo debido a la selección de la muestra en las predicciones derivadas de dicha muestra.

- Hay veces que, aunque se quiera tomar una muestra independiente, no es posible debido a la estructura implícita de la población. En estos casos se puede modelar utilizando procesos de estado discretos de Markov.

## Problemas fundamentales en Machine Learning

### Clustering

Si se tiene una matriz de datos / conjunto de datos $D$ de tamaño $n\times d$, se quiere lograr particionar a $D$ en grupos de filas similares.

### Clasificación y Regresión

**Clasificación**

Este problema está relacionado con el de clustering, pero en este caso los datos ya contienen información explícita de los grupos (hay etiqueta de grupo para cada fila). En este caso se quiere crear un modelo que, dada una observación nueva, prediga a qué grupo pertence (clasifique la nueva observación).

**Regresión**

En este problema, la variable, feature o característica que se quiere predecir es un numérica. Aparte de esto, es igual al problema de clasificación.

### Detección de outliers / valores atípicos

> Un valor atípico es una observación que se aleja tanto con respecto a las demás observaciones que se sospecha que fue generada por un mecanismo probabilístico diferente al de las demás observaciones.