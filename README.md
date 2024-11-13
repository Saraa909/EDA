# Análisis Exploratorio de Datos sobre el Cáncer de Mama
Autor: Sara González Rodríguez

## Descripción del Proyecto
Este proyecto realiza un análisis exploratorio del conjunto de datos de cáncer de mama, diseñado para identificar patrones y relaciones entre variables que pueden ser útiles para clasificar tumores como benignos o malignos. A través de técnicas de visualización y estadística descriptiva, se examinan diversas características de los tumores y se destacan las variables más relevantes para un diagnóstico efectivo.

## Archivo
- notebook.ipynb : cuaderno Jupyter con el EDA y los modelos de regresión.
- data.csv : Conjunto de datos de cáncer de mama utilizados en el análisis.
- README.md : Este archivo README.

## Análisis Realizado
Se exploraron varias características de los tumores, centrándose en variables como `radio_medio`, `perímetro_medio` y `área_medio`, que mostraron una alta dispersión, reflejando heterogeneidad en los tamaños de los tumores. La variable `textura_medio`, en cambio, demostró menor correlación con las demás, sugiriendo una contribución única en el análisis.

Los gráficos de dispersión y los diagramas de caja revelaron la presencia de valores atípicos en múltiples variables, lo que podría influir en futuros modelos si no se gestionan correctamente. Además, los tumores malignos tienden a presentar valores más altos en `radio_medio` y `textura_medio`, lo que indica su potencial para diferenciar tumores malignos de benignos, aunque la superposición de valores muestra que estos atributos no son suficientes por sí solos para una clasificación precisa.

## Distribución de Clases y Observaciones
En el conjunto de datos, el 62.7% de los tumores son benignos y el 37.3% son malignos, creando un desequilibrio en las clases. Este aspecto es crucial al construir modelos de clasificación para evitar sesgos hacia la clase predominante. También se observó que los tumores de mayor tamaño tienden a ser malignos, lo cual subraya la importancia de características como `radio`, `perímetro` y `área` en la predicción, aunque será necesario emplear modelos más avanzados para capturar de manera efectiva las interacciones entre estas variables.

## Conclusiones
Este análisis proporciona una base sólida para desarrollar modelos de aprendizaje automático que mejoren la detección temprana y la clasificación precisa de tumores malignos y benignos. Se recomienda aplicar técnicas de balanceo de clases y gestionar los valores atípicos para mejorar la precisión y robustez de los modelos predictivos.
