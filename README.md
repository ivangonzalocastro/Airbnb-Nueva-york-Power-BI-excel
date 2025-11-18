# Airbnb-Nueva-york-Power-BI-excel
Normalización, modelado y visualización para entender precios, reputación y disponibilidad en NYC

## Descripción General
Este proyecto analiza miles de alojamientos de **Airbnb en Nueva York**, utilizando Excel para limpiar y normalizar el dataset original, y Power BI para modelar los datos, crear relaciones, desarrollar medidas en DAX y construir un dashboard interactivo orientado a la toma de decisiones.
El objetivo fue responder preguntas sobre **precio, ubicación, reputación del alojamiento, flexibilidad del host y disponibilidad**, construyendo un análisis diagnóstico que ayuda a cualquier usuario de Airbnb a entender cómo varían los alojamientos según zona, tipo y calidad.

## Objetivos del Proyecto
Identificar cómo varía el precio en función del **barrio**, el **tipo de habitación** y las **políticas del host**.
Analizar la **calidad y reputación** de los alojamientos según puntuaciones, reviews y zonas.
Comprender la disponibilidad anual, cantidad de noches mínimas y restricciones comunes.
Crear visualizaciones interactivas para un usuario final sin conocimientos técnicos.

## Herramientas & Habilidades Utilizadas
### Excel
* Normalización del dataset original.
* Limpieza de valores y formatos.
* Uso de **VLOOKUP** y **XLOOKUP** para unir tablas satélite (neighbourhoods, room types, cancellation policies, etc.).
* Estandarización de columnas con fechas, tipos numéricos y textos.
### Power BI
* Modelado de datos mediante un Diagrama **Entidad–Relación** (tablas satélite + tabla fact TB_List).
* Transformaciones avanzadas en Power Query: tipo de datos, remover errores, reemplazo de símbolos, filtrados, ordenamientos y limpieza profunda.
* Creación de **medidas DAX** clave:
 * Precios máximo/mínimo/promedio
 * Promedio de disponibilidad
 * Promedio de puntuación
 * Moda de barrios
 * Conteo de alojamientos
* Diseño de dashboard profesional dividido en:
**Análisis por Barrio, Calidad y Reputación, Reglas de Reserva y Disponibilidad.**
Tooltips personalizados (host verificado, puntuación, precio promedio).
* Visuales usados:
**mapas, barras, dispersión, tarjetas, tablas dinámicas, segmentadores, KPIs.**

## Modelado (ERD)
Diseñé un modelo basado en:
* TB_List (tabla principal – alojamientos)
* TB_Neighbourhood_Group
* TB_Neighbourhood
* TB_Room_Type
* TB_Cancellation
* TB_Verified
Estas tablas se integraron en un esquema tipo estrella, optimizado para análisis de precios y reputación.

## Secciones del Dashboard
### 1. Análisis por Barrio
* Precio promedio por zona y barrio.
* Disponibilidad anual y tipo de habitación predominante.
* Identificación de zonas premium vs. económicas.
<img width="954" height="534" alt="Analisis por barrio" src="https://github.com/user-attachments/assets/8e98bb08-3828-4405-9bac-5f5570894167" />

### 2. Calidad y Reputación
* Puntuación promedio por barrio.
* Relación precio vs. reviews (gráfico de dispersión).
* Zonas con mayor volumen de opiniones reales.
<img width="957" height="538" alt="Calidad y Reputación" src="https://github.com/user-attachments/assets/8992aef1-b485-46bc-86f8-4bb025e0883b" />

### 3. Reglas de Reserva & Disponibilidad
* Noches mínimas requeridas.
* Políticas de cancelación predominantes.
* Porcentaje de hosts verificados por zona.
<img width="1034" height="585" alt="Reglas de reserva y disponibilidad" src="https://github.com/user-attachments/assets/21dd9f37-5b60-41a7-8a8c-37c0643db871" />
