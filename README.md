<h1 align="center"> House Prices Prediction </h1>

### Descripción del proyecto.

Este proyecto es uno de los desafios de Kaggle ["House Prices - Advanced Regression Techniques"](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques).
El objetivo principal del proyecto fue desarrollar un modelo que predijera los precios de viviendas, eligiendo un modelo basado en Random Forest Regression.

### Exploración inicial.

Se analizaron los datos del archivo **train.csv** para identificar:

* Valores nulos.
* Outliers.
* Variables categóricas.

Y conocer la estructura y caracteristicas de los datos.

### Tratamiento de valores nulos.

Se usaron técnicas de imputación como la mediana, None para indicar la ausencia de alguna característica de las viviendas como la mampostería, la moda o usamos 0 en variables numéricas
para indicar que no existe esa característica. También se eliminaron las columnas que tenían más del 80% de sus registros nulos.

### Análisis de Outliers.

Los valores atípicos encontrados en los datos eran representativos de casos raros pero reales del mercado inmobiliario. Se decidió incluirlos en el entrenamiento del modelo para
conservar la información de casos atípicos que podrían influir en el modelo.

### Transformación de variables categóricas.

Para que el modelo pudiera manejar variables categóricas, usamos la técnica de codificación One-Hot Encoding. Gracias a esto, aseguramos la homogeneidad entre los conjuntos de entrenamiento
y prueba junto con la inclusión de todas las posibles categorías en las variables transformadas.

### Selección del algoritmo.

Elegimos un modelo de regresión basado en Random Forest porque su capacidad para manejar datos con outliers y variables categóricas son muy robustas, también por su buen rendimiento sin necesidad
de extensiva normalización.

### Entrenamiento del modelo.

**RMSE: 28355.54**

**R²: 0.90**

Los resultados indicaron que el modelo capturó el 90% de la varianza de los precios de las viviendas, esto hace que el modelo sea adecuado para el conjunto de prueba.

### Gráficos y Anáisis.

Durante el proyecto se generaron varios gráficos para visualizar las distribuciones de las variables y también para el desempeño del modelo:

* Boxplot para identificar outliers.
* Scatter plots para analizar relaciones entre variables.
* Feature Importancie del modelo para ver las variables más relevantes para la predicción de precios.
* Graficos de barra para ver la distribución de datos dentro de las variables.

### Analisis final:

Con un R² de 0.90, el modelo nos da predicciones confiables para evaluación de precios de viviendas. En el proyecto vimos la importancia del preprocesamiento de datos para
mejorar la calidad de los modelos predictivos.

Número:
