# Visión por Computadora I - Trabajo Práctico 2

Este repositorio contiene la resolución del segundo trabajo práctico de la materia Visión por Computadora I (CEIA - FIUBA).

**Integrantes:**
- Lucia T. Capon Paul
- Cesar Orellana
- Madrid, Martin
- Leandro Britez

---

## Contenidos del Proyecto

El trabajo se encuentra implementado en el notebook:

`detector.ipynb`

### 1. Detección de Máximo Enfoque

Implementación de la métrica FM (*Frequency Domain Image Blur Measure*) propuesta en el paper *Image Sharpness Measure for Blurred Images in Frequency Domain* para evaluar la nitidez de imágenes en el dominio de frecuencias.

### 2. Análisis sobre Video

Procesamiento frame a frame del video `focus_video.mov` para detectar automáticamente el punto de máximo enfoque y visualizar la evolución de la métrica a lo largo de la secuencia.

### 3. Análisis con ROI

Evaluación de la métrica FM sobre una región de interés (ROI) central equivalente al 10% del área total del frame y comparación con los resultados obtenidos sobre la imagen completa.

---

## Resultados

| Experimento | Frame máximo | FM máximo |
|------------|-------------|-----------|
| Frame completo | 109 | 0.028624 |
| ROI central 10% | 111 | 0.357706 |

---

## Requisitos

Para ejecutar el notebook se requieren las siguientes librerías de Python:

- numpy
- opencv-python (cv2)
- matplotlib

---

## Estructura de Archivos

`detector.ipynb`  
Notebook principal con la implementación del algoritmo y el análisis de resultados.

`focus_video.mov`  
Video utilizado para la detección automática del punto de máximo enfoque.

`ImageSharpnessMeasureforBlurredImagesinFrequency.pdf`  
Paper de referencia utilizado para la implementación de la métrica FM.
