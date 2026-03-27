# 🎮 Video Game Success Analysis

## 📌 Descripción
Este proyecto analiza datos históricos de videojuegos hasta 2016 para identificar los factores que determinan el éxito comercial de un juego.

Se consideran variables como ventas por región, plataforma, género y calificaciones de usuarios y críticos.

El objetivo es apoyar la toma de decisiones para campañas publicitarias en 2017.

---

## 🎯 Objetivo de negocio
Identificar qué características hacen que un videojuego tenga éxito para enfocar inversiones en productos con mayor potencial de ventas.

---

## 🧹 Limpieza de datos

Se realizaron las siguientes transformaciones:

- Conversión de nombres de columnas a minúsculas
- Ajuste de tipos de datos:
  - `year_of_release` → entero
  - `critic_score` → numérico
  - `user_score` → conversión de texto a numérico
- Reemplazo de valores `"TBD"` por `NaN`
- Manejo de valores faltantes sin imputación para evitar sesgos
- Creación de variable:
  - `total_sales` = suma de ventas globales

---

## 📊 Análisis exploratorio

### 📅 Tendencias por año
- Se identificó que los datos recientes son más relevantes para predicción
- Se filtró un periodo representativo para el análisis

### 🎮 Plataformas
- Las plataformas tienen un ciclo de vida definido
- Algunas plataformas desaparecen mientras nuevas emergen
- Se identificaron plataformas líderes

### ⭐ Reseñas vs Ventas
- Se encontró correlación entre calificaciones de críticos y ventas
- Las reseñas de usuarios tienen menor impacto

### 🕹️ Géneros
- Los géneros más populares no siempre son los más rentables
- Existen diferencias claras en desempeño por género

---

## 🌍 Análisis por región

Se analizaron tres mercados:
- Norteamérica (NA)
- Europa (EU)
- Japón (JP)

### Hallazgos:
- Preferencias distintas por región
- Diferencias en plataformas dominantes
- Impacto variable de la clasificación ESRB

---

## 🧪 Pruebas de hipótesis

### Hipótesis 1
- H0: Xbox One y PC tienen la misma calificación promedio
- H1: Son diferentes

### Hipótesis 2
- H0: Acción y Deportes tienen la misma calificación promedio
- H1: Son diferentes

### Método
- Prueba t de Student
- α = 0.05

---

## 📈 Conclusiones

- Las plataformas tienen ciclos de vida claros
- Las críticas profesionales influyen más en ventas
- Las preferencias cambian por región
- Los datos recientes son clave para predicción
- No todos los géneros generan el mismo nivel de ingresos

---

## 💡 Recomendaciones

- Enfocar campañas en plataformas activas y en crecimiento
- Priorizar géneros con mayor rentabilidad
- Adaptar estrategias por región
- Considerar el impacto de críticas profesionales

---

## 📁 Estructura del proyecto

📦 video-game-analysis  
 ┣ 📜 notebook.ipynb  
 ┣ 📊 games.csv  
 ┗ 📄 README.md  
