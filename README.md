# Predicción de riesgo de accidente cerebrovascular mediante clasificación

## Descripción
Este proyecto tiene como objetivo predecir la probabilidad de que un paciente sufra un accidente cerebrovascular (ACV) a partir de una serie de características clínicas, utilizando algoritmos de clasificación. El modelo principal implementado fue una regresión logística, complementada con otros clasificadores como bosques aleatorios y máquinas de soporte vectorial para comparar el desempeño.
Dado el contexto médico del problema, se dio especial énfasis al análisis de la matriz de confusión, priorizando la minimización de los falsos negativos, es decir, los casos en los que el modelo no detecta un riesgo de ACV cuando realmente existe. Esta consideración es crítica en el ámbito de la salud, donde una predicción errónea puede tener consecuencias graves.
El proyecto incluyó también el ajuste del umbral de clasificación para optimizar la sensibilidad del modelo, así como la evaluación de métricas como el recall, la precisión y la curva ROC. Los resultados permitieron obtener un modelo útil para apoyar decisiones médicas preventivas.

## Dataset
El dataset utilizado contiene registros clínicos de pacientes con variables relevantes para el diagnóstico de riesgo de ACV. Incluye características demográficas y clínicas, y el objetivo es predecir la ocurrencia o no de un ACV. (Aquí se puede incluir la fuente del dataset, número total de registros y principales variables usadas si se dispone de esa información.)

## Metodología  
1. Análisis exploratorio de datos (EDA): Se examinaron distribuciones, valores faltantes y relaciones entre variables para entender el comportamiento de los datos.
2. Limpieza y transformación de datos: Tratamiento de valores faltantes, codificación de variables categóricas y normalización si fue necesaria.
3. Modelado: Implementación de regresión logística como modelo principal, junto con bosques aleatorios y máquinas de soporte vectorial para comparar desempeño.
4. Ajuste del umbral de clasificación: Optimización para priorizar la sensibilidad y reducir falsos negativos, crucial para la aplicación médica.
5. Evaluación del modelo: Análisis de la matriz de confusión, cálculo de métricas (recall, precisión) y evaluación con curva ROC.

## Resultados
Se obtuvo un modelo con buen desempeño para apoyar decisiones médicas preventivas, destacando un recall elevado gracias al ajuste del umbral. Esto permite un diagnóstico preliminar efectivo de la probabilidad de sufrir un accidente cerebrovascular.

## Lecciones aprendidas
- Manejo del desbalance de clases en clasificación binaria
- Importancia de elegir la métrica adecuada según el contexto del problema
- Aplicación y ajuste de la curva ROC y umbral para mejorar sensibilidad
- Análisis profundo de la matriz de confusión para entender los tipos de error y sus implicaciones clínicas

## Tecnologías
Scikit-learn, Pandas, Numpy, Matplotlib, Seaborn

## Mejoras futuras
- Implementar y optimizar en profundidad los modelos alternativos (bosques aleatorios, SVM)
- Analizar e interpretar los coeficientes de la regresión logística e implementar descenso de gradiente
- Organizar mejor el flujo de trabajo mediante pipelines de procesamiento y modelado
- Incorporar visualizaciones interactivas para facilitar la interpretación clínica

---
