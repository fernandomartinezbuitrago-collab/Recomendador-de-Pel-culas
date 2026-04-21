# 🎬 Sistema de Recomendación de Películas: KNN vs. Contenido

Este proyecto desarrolla un sistema de recomendación híbrido utilizando el dataset de **MovieLens**. El objetivo es resolver la "parálisis por decisión" de los usuarios mediante sugerencias personalizadas basadas en sus gustos y en la calidad del contenido.

## 🚀 Resumen del Proyecto
He implementado y comparado dos enfoques principales:
1. **Filtrado Colaborativo (KNN):** Encuentra patrones de consumo basados en la "sabiduría de la masa".
2. **Filtrado Basado en Contenido:** Sugiere películas similares por género, optimizado con un filtro de calidad (Rating).

## 📊 Hallazgos del Análisis Exploratorio (EDA)
Una parte crítica del proyecto fue identificar la **"Cola Larga" (Long Tail)**. Descubrí que miles de películas tenían menos de 5 votos, lo que generaba ruido en las recomendaciones. 
* **Decisión técnica:** Filtramos el dataset para incluir solo películas con más de 50 votos, mejorando drásticamente la precisión del modelo.

## 🧠 Modelado y Resultados
* **KNN (K-Nearest Neighbors):** Logró identificar "clústeres" de películas de alta calidad. Al probar con *The Matrix*, el sistema sugirió con éxito clásicos de ciencia ficción como *Star Wars: Episode V*.
* **Basado en Contenido:** Se optimizó para que, dentro de un mismo género, el sistema priorice las películas con mejor puntuación media, evitando recomendar contenido irrelevante.

## 🛠️ Tecnologías utilizadas
* **Python** (Pandas, Numpy)
* **Scikit-learn** (NearestNeighbors, Cosine Similarity)
* **Matplotlib & Seaborn** (Visualización)

## 🎓 Créditos
Proyecto realizado como parte del Máster en Data Science en **ENAE Business School**. Agradecimientos especiales a mi profesor por el feedback técnico para optimizar los motores de recomendación.
