#  Proyecto Final de Machine Learning: Predicción de Riesgo Cardiovascular

Este repositorio contiene el pipeline completo de un proyecto de Machine Learning diseñado para predecir el riesgo de padecer enfermedades cardiovasculares en pacientes, basándose en parámetros médicos, físicos y de estilo de vida.

##  Descripción del Proyecto

El objetivo principal de este proyecto es aplicar, evaluar y comparar múltiples algoritmos de Machine Learning (supervisados y no supervisados) para encontrar el modelo más óptimo en la detección temprana de anomalías cardiovasculares. 

##  Tecnologías y Herramientas

* **Lenguaje:** Python 
* **Manipulación de Datos:** Pandas, NumPy
* **Machine Learning Clásico:** Scikit-Learn
* **Deep Learning:** TensorFlow / Keras
* **Visualización:** Matplotlib, Seaborn

##  Dataset y Preprocesamiento

Se utilizó el conjunto de datos `Cardiovascular Disease`. Antes del entrenamiento, los datos pasaron por un riguroso proceso de limpieza:
1. **Eliminación de Outliers:** Filtrado de valores atípicos imposibles (ej. alturas < 140cm, pesos < 40kg).
2. **Escalamiento:** Normalización de variables continuas utilizando `StandardScaler`.

##  Modelos Entrenados y Evaluados

Se implementaron los siguientes algoritmos para comparar su rendimiento:

1. **Regresión Logística:** Modelo base (baseline).
2. **Árbol de Decisión:** Configurado con una profundidad máxima para evitar el sobreajuste.
3. **Máquinas de Vectores de Soporte (SVM):** Utilizando un kernel radial (`rbf`).
4. **Red Neuronal Artificial:** Arquitectura de múltiples capas densas con función de activación sigmoide para clasificación binaria.
5. **K-Means (No Supervisado):** Agrupación en 2 clústeres para contrastar el aprendizaje no supervisado con las etiquetas reales.

##  Resultados y Visualizaciones

El análisis en el notebook incluye métricas detalladas (`Accuracy`, `Precision`, `Recall`, `F1-Score`) y visualizaciones clave:
* **Gráficos de Barras:** Para la comparativa general de métricas.
* **Matrices de Confusión:** Análisis a profundidad de los Verdaderos Positivos, Verdaderos Negativos y los márgenes de error.


Datos obtenidos de: https://www.kaggle.com/datasets/colewelkins/cardiovascular-disease/data 
