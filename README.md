# 🛰️ Robust Illuminance Drone Detection Using Modulo Images

Este repositorio contiene el código y los recursos asociados al trabajo de investigación **"Robust Illuminance Drone Detection Using Modulo Images"**, presentado en la **XXII Conferencia Colombiana de Tecnologías de la Información y Comunicaciones - STSIVA 2025**  
🔗 [Sitio oficial de STSIVA](https://stsiva.ieee.org.co/)

## 📌 Descripción

El objetivo principal de esta investigación es abordar el problema de la detección de drones en entornos con condiciones extremas de iluminación, donde los sensores tradicionales (CCD/CMOS) sufren de saturación y pérdida de información.

Para ello, se propone una metodología basada en imágenes *modulo*, capturadas con sensores *modulo-ADC*, que permiten preservar estructuras de la escena incluso en situaciones de sobreexposición. A diferencia de enfoques tradicionales que requieren reconstrucción HDR, este trabajo presenta un modelo **YOLOv11** ajustado directamente sobre imágenes modulo, logrando detección precisa con menor costo computacional.

## 🧠 Principales contribuciones

- ✅ Ajuste fino (*fine-tuning*) de **YOLOv11** sobre datos modulo sin reconstrucción HDR.
- ✅ Detección robusta de drones en distintos niveles de exposición (α = 1.5, 2, 3).
- ✅ Evaluación comparativa contra imágenes saturadas y reconstrucciones HDR (SPUD y AHFD).
- ✅ Reducción del tiempo de inferencia manteniendo alta precisión (F1-score > 91%).

## ⚙️ Tecnologías y herramientas

- Python 3.10+
- YOLOv11 (Ultralytics)
- Google Colab (GPU Tesla T4)
- Numpy, OpenCV, Matplotlib
- Dataset: [UAV Drone Dataset - Kaggle](https://www.kaggle.com/datasets/dasmehdixtr/drone-dataset-uav)

## 📊 Resultados

- F1-Score superior al 91% en condiciones de alta exposición.
- Rendimiento comparable con reconstrucciones HDR, pero con menor latencia.
- Modelo optimizado para despliegue en tiempo real.

## 📄 Publicación

> **Luis Toscano-Palomino**, Kebin Contreras, Brayan Monroy, Jorge Bacca  
> _Robust Illuminance Drone Detection Using Modulo Images_  
> **Conferencia STSIVA 2025**, IEEE Colombia
