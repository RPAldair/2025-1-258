# 1ACC0216--TB1-2025-1

![image](https://github.com/user-attachments/assets/61a731be-baf1-42a2-87e1-b8e63343da40)


1ACC0216-2510-258 - Fundamentos de Data Science · TB2

2025 · Ciencia de la Computación

Profesora: Nérida Isabel Manrique Tunque


# Metodología CRISP-DM: Tendencias de las estadísticas de videos de YouTube
## Índice
1. [Objetivo del proyecto](#objetivo-del-proyecto)  
2. [Descripción del dataset](#descripción-del-dataset)
3. [Conclusiones clave](#conclusiones-clave)  
4. [icencia](#licencia)

## 1. Objetivo del proyecto

Analizar un conjunto de datos de videos en tendencia de YouTube en Corea del Sur, con el fin de detectar patrones relevantes en el comportamiento de usuarios y creadores, así como identificar factores que influyen en la viralización de contenido. A partir del análisis exploratorio y la preparación de los datos, se desarrollan visualizaciones, métricas y un modelo predictivo que permita estimar interacciones como vistas, “me gusta” y comentarios.


---
### Grupo de trabajo:

Alzamora Gonzales Leonel         -     U20231c427@upc.edu.pe(Business Project Sponsor)

Fabian Marcelo, Rojas Cuadros    -     U202218498@upc.edu.pe(Data Analyst)

Avalos Sánchez, César Gabriel    -     U202310307@upc.edu.pe(Data Scientist)

Rivas Pinto, Piero Aldair        -     U202122405@upc.edu.pe(Data Engineer)

---
## 2. Descripción del dataset

El dataset reúne información detallada sobre reservas de hotel, incluyendo datos del cliente, categoría de habitación, fechas de ingreso, duración de la estancia y otros elementos clave de cada transacción. Cada fila corresponde a una reserva individual e incluye múltiples atributos que permiten analizar los factores que afectan la demanda en el sector hotelero.

Los datos utilizados, son una versión modificada para el proyecto, tienen como base el conjunto de datos proviene del portal Kaggle e incluye videos en tendencia en Corea del Sur durante 2021. Contiene variables como:

- `video_id`, `title`, `channel_title`
- Métricas de interacción: `views`, `likes`, `dislikes`, `comment_count`
- Fecha de publicación (`publish_time`) y de tendencia (`trending_date`)
- Variables geográficas (`state`, `lat`, `lon`)
- Variables categóricas (`category_id`, `category_name`)
- Indicadores de estado (`comments_disabled`, `ratings_disabled`, etc.)

[Diccionario de Datos]

## 3. Conclusiones clave

El análisis de datos de YouTube en Corea del Sur permitió identificar categorías, canales y variables que influyen en el rendimiento y viralización de los videos. Las categorías más frecuentes en tendencias fueron Entertainment y Music, aunque Education presentó una proporción positiva superior en términos de interacción (likes / dislikes).

Se creó un pipeline de preparación de datos robusto que incluyó detección y tratamiento de outliers, imputación de valores faltantes, normalización y codificación de variables categóricas. Esto permitió trabajar con un dataset limpio, estructurado y apto para modelado.

A partir del análisis exploratorio y el tratamiento de datos, se identificaron insights clave, como el hecho de que los videos más vistos no siempre coinciden con los más comentados, y que los canales más frecuentes en tendencia no necesariamente son los más valorados por los usuarios.

Se construyó un modelo de regresión para predecir la cantidad de "likes" a partir de otras variables numéricas y categóricas, logrando un desempeño aceptable. Esto demuestra la posibilidad de estimar métricas clave antes de que un video alcance su punto máximo de difusión.

Durante el proyecto se experimentaron varios desafíos, como la alta proporción de valores faltantes en columnas temporales (trending_date, days_to_trending) y la presencia de registros duplicados. Estas dificultades fueron superadas gracias a un enfoque iterativo de limpieza, revisión de decisiones y aplicación disciplinada de la metodología CRISP-DM.

El trabajo interdisciplinario y la especialización de roles (Data Engineer, Data Scientist, Data Analyst y Líder de Proyecto) permitió abordar cada etapa del proceso con profundidad. Se comprobó que la preparación de datos es una fase crítica que impacta directamente en la calidad de los modelos y visualizaciones generadas.

---

## Licencia

El presente trabajo está publicado bajo la licencia [MIT](LICENSE).
