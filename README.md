# SAT-Python
Entrega del trabajo de python- Nicolás Udry y Benjamín Ochoa Mabres
```markdown
# Análisis de Depresión en Estudiantes
# Link al dataset: https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset 
## Introducción

Este proyecto se centra en el análisis de un conjunto de datos sobre la depresión en estudiantes. El objetivo principal es identificar patrones, posibles factores de riesgo y relaciones entre diversas variables que puedan influir en el bienestar emocional de esta población. El análisis exploratorio inicial sentó las bases para comprender la estructura del dataset, manejar valores faltantes, analizar variables numéricas y categóricas, y detectar posibles valores atípicos. Este trabajo busca proporcionar una visión integral y preventiva sobre el problema de la depresión en estudiantes, explorando la relación entre factores individuales y académicos con indicadores de salud mental.

## Manejo de Outliers

Se realizó una consideración especial sobre los valores atípicos en el dataset. Se identificaron dos variables clave:

* **CGPA (Cumulative Grade Point Average):** Se reconoció que este valor se encuentra inherentemente limitado a una escala específica (0 a 4.00 o 5.00), por lo que los valores dentro de este rango no se consideraron atípicos.
* **Job Satisfaction:** Esta variable, al depender de un sentimiento subjetivo, presenta una variabilidad natural que no se consideró anómala. Además, con solo 8 datos identificados como posibles outliers, y al no tratarse de un análisis predictivo donde estos podrían influir significativamente en la columna objetivo, se decidió no realizar ningún tratamiento sobre estos valores.

En conclusión, no se aplicaron técnicas de tratamiento de outliers debido a la naturaleza de las variables mencionadas y el enfoque exploratorio del análisis inicial.

## Visualizaciones

### Análisis de Distribución del Dataset

Se utilizaron gráficos de pastel para visualizar la distribución general de las siguientes variables:

* Porcentaje de estudiantes por género.
* Proporción de estudiantes con antecedentes familiares de enfermedad mental.
* Porcentaje de estudiantes que reportaron haber tenido pensamientos suicidas.
* Distribución de las horas de sueño de los estudiantes.

### Visualización de Variables Categóricas

Se analizó la frecuencia de diversas variables categóricas y se calculó la frecuencia relativa de la variable "Depresión" en función de las categorías de otras variables, incluyendo:

* Género
* Ciudad
* Profesión
* Duración del Sueño
* Dieta
* Grado de Estudios
* Pensamientos Suicidas
* Estrés Financiero
* Historia de Salud Mental

Este análisis reveló patrones importantes, como una proporción similar de depresión entre géneros (58%), una mayor prevalencia de depresión en estudiantes con menos de 5 horas de sueño y una fuerte relación entre una dieta no saludable y la depresión. El estrés financiero también mostró una correlación significativa con la depresión, mientras que el historial familiar de problemas de salud mental presentó una correlación menos marcada.

### Mapa de Distribución Geográfica

Se generó un mapa para visualizar la distribución geográfica de los casos de depresión entre los estudiantes en las diferentes ciudades del dataset. El tamaño de los círculos en el mapa es proporcional al número de casos de depresión registrados en cada ciudad, facilitando la identificación de posibles concentraciones geográficas.

### Matriz de Correlación y Mapa de Calor (Variables Numéricas)

Se utilizó una matriz de correlación y un mapa de calor para examinar las relaciones entre las variables numéricas del dataset. Los hallazgos más destacados incluyeron una correlación de 0.77 entre la presión y la satisfacción en el trabajo, y una correlación de 0.47 entre la presión académica y la depresión.

### Mapa de Calor (Variables Categóricas y Depresión)

Se empleó un mapa de calor para analizar la relación entre variables categóricas y la presencia de depresión, combinando información relativa (porcentajes) y absoluta (frecuencia de casos). Esta visualización permitió identificar proporciones significativas de depresión dentro de cada categoría, complementando el análisis de gráficos de barra previo.

## Modelos de Machine Learning

### Regresión Logística

El modelo de regresión logística demostró un rendimiento sólido en la identificación de estudiantes con y sin depresión, clasificando correctamente a 3342 personas con depresión y 1921 sin ella. A pesar de presentar algunos falsos negativos y positivos, se considera una herramienta útil para predecir escenarios preventivos y de seguimiento psicológico.

### Árbol de Decisión

El modelo de árbol de decisión logró una precisión general del 66%, clasificando correctamente a 2879 personas con depresión y 1725 sin ella. Si bien útil para detectar la mayoría de los casos con síntomas, su precisión no se consideró óptima para este contexto.

### Random Forest

El modelo de Random Forest, una técnica de ensamble, alcanzó un buen accuracy del 72% con métricas de precisión, recall y F1-score equilibradas para ambas categorías de depresión. El análisis de importancia de variables indicó que el CGPA fue la variable más influyente, seguida por la presión académica, la edad y las horas de estudio.

## Conclusión

Este análisis proporcionó información valiosa sobre los factores asociados a la depresión en estudiantes. Se identificaron patrones significativos en variables demográficas, hábitos y condiciones académicas. La duración del sueño, la dieta, la presión académica y el rendimiento escolar emergieron como factores importantes. Los modelos de machine learning, especialmente la regresión logística y Random Forest, ofrecen herramientas prometedoras para estrategias de prevención y seguimiento psicológico, al permitir mapear la influencia de diversas variables en la probabilidad de depresión. Este trabajo subraya el potencial del análisis de datos para abordar problemas de salud mental de manera preventiva e integral.
```
