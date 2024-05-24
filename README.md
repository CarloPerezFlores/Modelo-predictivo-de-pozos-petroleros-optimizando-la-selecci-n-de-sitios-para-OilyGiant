# Modelo-predictivo-de-pozos-petroleros-optimizando-la-selección-de-sitios-para-OilyGiant
En este proyecto se utiliza análisis de datos y técnicas de machine learning para seleccionar las mejores ubicaciones para abrir 200 nuevos pozos petroleros en tres regiones diferentes.


**<span style="font-size:20px; font-weight:bold;">Descripción</span>**

El proyecto consiste en emplear análisis de datos y técnicas de machine learning para evaluar y comparar diferentes ubicaciones en tres regiones para la apertura de nuevos pozos petroleros. Se utilizan modelos de regresión lineal para predecir el volumen de reservas en cada ubicación, y se calcula el beneficio potencial y el riesgo de pérdidas para cada región. La región seleccionada será aquella con el mayor beneficio promedio y un riesgo de pérdidas inferior al 2.5%.

**<span style="font-size:20px; font-weight:bold;">Contenido</span>**

-datos_region1.csv, datos_region2.csv, datos_region3.csv: Archivos CSV que contienen los datos de las tres regiones.

-analisis_exploratorio.ipynb: Jupyter Notebook con el análisis exploratorio de datos.

-modelo_regresion_lineal.ipynb: Jupyter Notebook con el entrenamiento del modelo de regresión lineal y la evaluación del mismo.

-calculadora_beneficio_riesgo.ipynb: Jupyter Notebook con el cálculo del beneficio potencial y el riesgo de pérdidas, y la selección de la región óptima.

**<span style="font-size:20px; font-weight:bold;">Requisitos</span>**

## Python 3
## Jupyter Notebook
## Pandas
## NumPy
## Matplotlib
## Seaborn
## Plotly
## scikit-learn

**<span style="font-size:20px; font-weight:bold;">Preparación de datos:</span>**

Se descargarán y prepararán los datos de exploración geológica de las tres regiones (geo_data_0.csv, geo_data_1.csv, geo_data_2.csv). Esto incluirá la limpieza de datos y la comprensión de las características relevantes.

**<span style="font-size:20px; font-weight:bold;">Entrenamiento y evaluación del modelo:</span>**

Para cada región, se dividirán los datos en conjuntos de entrenamiento y validación.
Se utilizará regresión lineal para entrenar un modelo que prediga el volumen de reservas en los nuevos pozos.
Se evaluará el modelo utilizando métricas como el RMSE (Error Cuadrático Medio) y el volumen medio de reservas predicho.

**<span style="font-size:20px; font-weight:bold;">Preparación para el cálculo de ganancias:</span>**

Se almacenarán los valores necesarios para los cálculos en variables separadas.
Se comparará el valor medio de reservas predicho con el umbral necesario para evitar pérdidas.

**<span style="font-size:20px; font-weight:bold;">Cálculo de ganancias para la selección de pozos petroleros:</span>**

Se seleccionarán los 200 pozos con los valores de predicción más altos para cada región.
Se calculará la ganancia potencial de estos 200 pozos principales para cada región.

**<span style="font-size:20px; font-weight:bold;">Cálculo de riesgos y ganancias para cada región:</span>**

Se empleará la técnica de bootstrapping con 1000 muestras para encontrar la distribución de los beneficios.
Se calcularán el beneficio promedio, el intervalo de confianza del 95% y el riesgo de pérdidas para cada región.
Al finalizar estos pasos, se podrá proponer una región para el desarrollo de pozos petroleros basada en el análisis de ganancias y riesgos. Es importante destacar que se utilizará únicamente la regresión lineal para el entrenamiento del modelo y que se aplicarán criterios específicos para garantizar la rentabilidad y minimizar los riesgos asociados con la inversión en los nuevos pozos petroleros.



