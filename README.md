# Clasificación de Cáncer de Mama con Machine Learning

## 📌 Contexto

El cáncer de mama es el tipo de cáncer más prevalente en el mundo. En 2020, se diagnosticó a 2,3 millones de mujeres y causó la muerte de aproximadamente 685.000. Su detección temprana y tratamiento adecuado pueden marcar una gran diferencia en la supervivencia, especialmente en países de ingresos bajos y medianos donde las tasas de mortalidad siguen siendo altas.

## 🎯 Objetivo

Desarrollar un modelo de clasificación de cáncer de mama que supere el umbral del 95% en las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-score

El objetivo es detectar de forma fiable los casos de cáncer maligno a partir de datos clínicos utilizando técnicas de machine learning.

## 📊 Dataset

El dataset proviene del repositorio de la UCI (Wisconsin Breast Cancer Dataset), accesible públicamente desde:

👉 [Enlace al dataset y columnas](https://github.com/nodd3r/recursos/tree/main/datasets/cancer)

El dataset incluye características como:

- Grosor del grupo celular
- Tamaño y forma celular uniforme
- Adhesión marginal
- Tamaño de célula epitelial
- Cromatina suave
- Núcleos normales
- Mitosis
- ...entre otros

## 🧪 Metodología

1. **Carga y limpieza de datos**
   - Reemplazo de valores nulos representados con `'?'`
   - Conversión de tipos y codificación de etiquetas

2. **Análisis exploratorio**
   - Estadísticas descriptivas
   - Visualizaciones para detectar patrones y distribución de clases

3. **Preprocesamiento**
   - Balanceo de clases (si es necesario)
   - División en subconjuntos de entrenamiento y test con estratificación

4. **Modelado**
   - Se probaron distintos clasificadores:
     - Regresión logística
     - Árboles de decisión
     - KNN
     - Naive Bayes
     - SVM
     - Random Forest
   - Optimización de hiperparámetros

5. **Evaluación**
   - Se seleccionó el mejor modelo que cumplía con **score, accuracy, precision, recall y f1-score ≥ 0.95**

## ✅ Resultados

El modelo final superó todas las métricas requeridas:

- Accuracy: ≥ 0.95
- Precision: ≥ 0.95
- Recall: ≥ 0.95
- F1-score: ≥ 0.95

## 🧠 Modelo final

El clasificador seleccionado fue:

```python
modelo_definitivo = <nombre_del_modelo>
````
Sustituye <nombre_del_modelo> por el modelo que mejor rendimiento ofreció (por ejemplo: RandomForestClassifier()).

## 🚀 Requisitos
Puedes instalar las dependencias con:
````bash
pip install -r requirements.txt
````
## 📁 Estructura del proyecto

├── cancer_classification.ipynb

├── README.md

├── requirements.txt

├── .gitignore

└── data/

## 🏁 Cómo ejecutar
1. Clona el repositorio

2. Ejecuta el Jupyter Notebook paso a paso

3. Entrena y evalúa modelos

4. Ajusta hiperparámetros si es necesario

5. Verifica que las métricas cumplan con los requisitos

## ✍️ Autor
Proyecto de aprendizaje aplicado con datos reales del cáncer de mama.
