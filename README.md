# ⚽ Minería de Datos: Análisis Histórico de la Premier League (2000 - 2025)

## 📋 Información del Proyecto
* **Integrantes:** Vicente Canio - Alonso Escobar
* **Docente:** Carlos Muñoz
* **Dataset:** [English Premier League (EPL) Match Data 2000-2025](https://www.kaggle.com/datasets/marcohuiii/english-premier-league-epl-match-data-2000-2025)

## 📝 Descripción
Este proyecto realiza un **Análisis Exploratorio de Datos** exhaustivo sobre el historial de partidos de la Premier League inglesa. El objetivo es identificar patrones tácticos, cuantificar la ventaja de jugar en casa y determinar qué factores estadísticos (tiros, faltas, tarjetas) tienen una correlación directa con el éxito en el marcador final.

## 🚀 Fases del Proyecto

### 1. Importación y Carga de Datos
* Configuración del entorno de trabajo utilizando librerías esenciales como **Pandas, NumPy, Matplotlib y Seaborn**.
* Carga y verificación de las dimensiones del dataset histórico (`epl_final.csv`), que cuenta con 9380 registros y 22 columnas iniciales.

### 2. Entendimiento Inicial de los Datos
* Inspección de tipos de datos para asegurar la consistencia entre variables categóricas y numéricas.
* Validación de la integridad del dataset mediante la búsqueda y confirmación de ausencia de valores nulos.
* Generación de resúmenes estadísticos iniciales para comprender la distribución de resultados y los equipos con mayor presencia histórica.

### 3. Limpieza y Transformación
* **Procesamiento Temporal:** Conversión de la columna `MatchDate` a formato *datetime* y extracción de nuevas variables de Año y Mes para análisis de tendencias estacionales.
* **Codificación de Datos:** Aplicación de `LabelEncoder` para transformar resultados de texto (H, A, D) en valores numéricos, permitiendo su procesamiento en modelos estadísticos.

### 4. Análisis Exploratorio de Datos
* **Análisis de Resultados:** Visualización de la probabilidad histórica de victoria local, visitante y empate mediante gráficos de pastel y barras.
* **Dinámica del Juego:** Estudio del impacto del resultado al medio tiempo en el desenlace final del partido.
* **Evolución Histórica:** Seguimiento de la producción de goles y la efectividad de la localía a lo largo de las décadas (temporada 2000/01 a 2024/25).
* **Métricas Disciplinarias:** Identificación de los equipos con mayor acumulación histórica de faltas y tarjetas (amarillas y rojas).

### 5. Detección de Outliers y Matriz de Correlación
* **Análisis de Distribución:** Uso de *Boxplots* para detectar valores atípicos en variables clave como tiros totales, tiros a puerta y faltas cometidas.
* **Análisis de Correlación:** Construcción de una matriz de correlación visualizada con un mapa de calor (*Heatmap*) para determinar el peso de cada variable estadística en el resultado final del encuentro.

---
## 🛠️ Tecnologías Utilizadas
* **Python:** Lenguaje principal de programación.
* **Pandas & NumPy:** Manipulación y limpieza de datos.
* *Matplotlib & Seaborn:** Visualización de datos avanzada.
