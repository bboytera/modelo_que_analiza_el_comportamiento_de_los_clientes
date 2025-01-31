# Modelo_que_analiza_el_comportamiento_de_los_clientes
Este es un modelo que analiza el comportamiento de los clientes y recomienda uno de los nuevos planes de una compañia movil
# Introducción
La compañía móvil Megaline no está satisfecha al ver que muchos de sus clientes utilizan planes heredados. Quieren desarrollar un modelo que pueda analizar el comportamiento de los clientes y recomendar uno de los nuevos planes de Megaline: Smart o Ultra.

Tenemos acceso a los datos de comportamiento de los suscriptores que ya se han cambiado a los planes nuevos. 

Nota: los datos ya se encuentran preprocesados!
# Descripción de los datos
Los datos se encuentran en el archivo 'users_behavior.csv'.

Cada observación en el dataset contiene información del comportamiento mensual sobre un usuario. La información dada es la siguiente:

- сalls — número de llamadas,
- minutes — duración total de la llamada en minutos,
- messages — número de mensajes de texto,
- mb_used — Tráfico de Internet utilizado en MB,
- is_ultra — plan para el mes actual (Ultra - 1, Smart - 0).
# Habilidades y herramientas técnicas
- Python
- Pandas
- Matplotlib
- Scikit-learn
- Machine Learning
# Conclusión
Los resultados obtenidos al evaluar los tres modelos de machine learning (Árbol de Decisión, Bosque Aleatorio y Regresión Logística) proporcionan una visión clara de su rendimiento en la tarea específica planteada.

La curva ROC y la curva de Precision-Recall son herramientas esenciales para esta evaluación. En términos de la **curva ROC, el Bosque Aleatorio** obtuvo el mejor rendimiento con un **AUC de 0.76**, seguido por el Árbol de Decisión con un AUC de 0.69, y por último la Regresión Logística con un AUC de 0.64. Esto indica que el Bosque Aleatorio es más eficaz en distinguir entre clases positivas y negativas.

Por otro lado, en la curva de **Precision-Recall, el Bosque Aleatorio** también demostró ser el modelo más robusto con un **AP de 0.65**, en comparación con el AP de 0.54 de la Regresión Logística y el AP de 0.51 del Árbol de Decisión. Estos resultados sugieren que el Bosque Aleatorio mantiene un equilibrio más favorable entre precisión y recall, lo que es crucial en situaciones donde la clase positiva es de particular interés.

En resumen, el **Bosque Aleatorio** se presenta como el modelo más adecuado para este conjunto de datos y problema específico, ofreciendo un balance superior en términos de precisión y capacidad de detección.

