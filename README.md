# Movilidad Urbana y Productividad Económica en Latinoamérica 2024 – Análisis Sprint 5

Este repositorio contiene el análisis de datos desarrollado para evaluar cómo la movilidad urbana (congestión y tiempos de viaje) se relaciona con la productividad económica (PIB per cápita) en las principales ciudades latinoamericanas.

El proyecto combina fuentes de datos de **TomTom Traffic Index** y **OECD Cities Economy**, integrando procesos de limpieza de datos, estandarización de formatos, unión de tablas (*inner join*) y visualización de distribuciones y outliers para la toma de decisiones estratégicas [cite: 11].

## 📂 Contenido del repositorio

- `notebooks/`
  → Contiene el Jupyter Notebook principal con la carga, la limpieza, el EDA, las uniones y los resúmenes ejecutivos.
- `ladb_mobility_economy_2024_clean.csv`
  → Dataset final limpio y consolidado listo para análisis o tableros de visualización.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Tb5gkOJXsKlWYLJH9ebVOnOFA96EoGVJ?usp=sharing)

O:

1. Abre el archivo `.ipynb` en este repositorio de GitHub.
2. Haz clic en el botón **Open in Colab** en la parte superior del visor de GitHub.

## 📘 Cómo reproducir el análisis

1. Clona este repositorio o descarga los archivos.
2. Abre el notebook en Google Colab o en tu entorno local de Jupyter.
3. Ejecuta las celdas en orden secuencial.
4. Asegúrate de que las rutas de los archivos fuente (`/datasets/tomtom_traffic.csv` y `/datasets/oecd_city_economy.csv`) estén disponibles en tu entorno de trabajo.

## 🧠 Objetivos y Hallazgos Clave

- **Calidad de datos:** Estandarización de nombres de columnas a `snake_case`, conversión de campos de fecha (`datetime`) y sanitización de variables numéricas con separadores especiales y porcentajes.
- **Movilidad:** Identificación de patrones de tráfico anuales, destacando a la **Ciudad de México** y **Tokio/Bogotá** en los índices de retraso por congestión (`jams_delay`).
- **Relación Socioeconómica:** Cruce de información mediante uniones relacionales para evaluar cuellos de botella de infraestructura y su impacto en la competitividad urbana, identificando a **Bogotá** como una zona prioritaria de inversión debido a su alta congestión en relación con su productividad.
