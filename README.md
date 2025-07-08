# 1ACC0216--TB1-2025-1

![image](https://github.com/user-attachments/assets/61a731be-baf1-42a2-87e1-b8e63343da40)


1ACC0216-2510-258 - Fundamentos de Data Science · TB2

2025 · Ciencia de la Computación

Profesora: Nérida Isabel Manrique Tunque


# Metodología CRISP-DM: Tendencias de las estadísticas de videos de YouTube
## Índice
1. [Objetivo del proyecto](#objetivo-del-proyecto)
2. [Integrantes del grupo](#grupo-de-trabajo)
3. [Descripción del dataset](#3-descripción-del-conjunto-de-datos)
4. [Conclusiones](#4-conclusiones-clave)  
5. [icencia](#licencia)

## 1. Objetivo del proyecto

Analizar un conjunto de datos de videos en tendencia de YouTube en Corea del Sur, con el fin de detectar patrones relevantes en el comportamiento de usuarios y creadores, así como identificar factores que influyen en la viralización de contenido. A partir del análisis exploratorio y la preparación de los datos, se desarrollan visualizaciones, métricas y un modelo predictivo que permita estimar interacciones como vistas, “me gusta” y comentarios.


---
### 2. Grupo de trabajo:

Alzamora Gonzales Leonel         -     U20231c427@upc.edu.pe(Business Project Sponsor)

Fabian Marcelo, Rojas Cuadros    -     U202218498@upc.edu.pe(Data Analyst)

Avalos Sánchez, César Gabriel    -     U202310307@upc.edu.pe(Data Scientist)

Rivas Pinto, Piero Aldair        -     U202122405@upc.edu.pe(Data Engineer)

---
## 3. Descripción del conjunto de datos



Los datos utilizados, son una versión modificada para el proyecto, tienen como base el conjunto de datos proviene del portal Kaggle e incluye videos en tendencia en Corea del Sur durante 2021. El dataset reúne información detallada sobre estadísticas de videos en tendencia en Corea del Sur durante 2021 como:

- `video_id`, `title`, `channel_title`
- Métricas de interacción: `views`, `likes`, `dislikes`, `comment_count`
- Fecha de publicación (`publish_time`) y de tendencia (`trending_date`)
- Variables geográficas (`state`, `lat`, `lon`)
- Variables categóricas (`category_id`, `category_name`)
- Indicadores de estado (`comments_disabled`, `ratings_disabled`, etc.)

[Ver diccionario de datos (PDF)](../data/Diccionario de Datos.pdf)

## 4. Conclusiones

El modelo de Árbol de Regresión permitió predecir con alta precisión la cantidad de vistas que puede alcanzar un video en YouTube dentro del contexto de Corea del Sur, alcanzando un R² de 0.992 en el conjunto de prueba.

Las variables que más influyeron en las predicciones fueron dislikes, comment_ratio y comment_count, lo que sugiere que la participación del público (en forma de comentarios o reacciones) tiene un fuerte impacto en la visibilidad de un video.

La diferencia mínima entre el R² del entrenamiento (0.997) y el de prueba (0.992) indica que el modelo predice correctamente y no está sobreajustado, por lo que puede utilizarse con confianza para nuevos datos.

La preparación y limpieza del dataset, junto con la creación de variables derivadas como like_ratio y comment_ratio, fueron factores clave para mejorar la capacidad predictiva del modelo.

La visualización de los datos y el análisis exploratorio fueron fundamentales para entender el comportamiento de las variables y justificar el uso del modelo elegido.


---

## Licencia

El presente trabajo está publicado bajo la licencia [MIT](LICENSE).
