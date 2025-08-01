# 🛰️ Robust Illuminance Drone Detection Using Modulo Images

This repository contains the code and resources for the research work **"Robust Illuminance Drone Detection Using Modulo Images"**, presented at the **XXII Colombian Conference on Information and Communication Technologies - STSIVA 2025**  
🔗 [Official STSIVA Website](https://stsiva.ieee.org.co/)

## 📌 Description

The main objective of this research is to address the problem of drone detection in environments with extreme lighting conditions, where traditional sensors (CCD/CMOS) suffer from saturation and information loss.

To tackle this, we propose a methodology based on *modulo images*, captured with *modulo-ADC* sensors, which preserve scene structures even under overexposure. Unlike traditional approaches that require HDR reconstruction, this work presents a **YOLOv11** model fine-tuned directly on modulo images, achieving accurate detection with lower computational cost.

## 🧠 Main Contributions

- ✅ Fine-tuning of **YOLOv11** on modulo data without HDR reconstruction.
- ✅ Robust drone detection at different exposure levels (α = 1.5, 2, 3).
- ✅ Comparative evaluation against saturated images and HDR reconstructions (SPUD and AHFD).
- ✅ Reduced inference time while maintaining high accuracy (F1-score > 91%).

## ⚙️ Technologies and Tools

- Python 3.10+
- YOLOv11 (Ultralytics)
- Google Colab (Tesla T4 GPU)
- Numpy, OpenCV, Matplotlib
- Dataset: [UAV Drone Dataset - Kaggle](https://www.kaggle.com/datasets/dasmehdixtr/drone-dataset-uav)

## 📊 Results

- F1-Score above 91% under high exposure conditions.
- Performance comparable to HDR reconstructions, but with lower latency.
- Model optimized for real-time deployment.

## 📄 Publication

> **Luis Toscano-Palomino**, Kebin Contreras, Brayan Monroy, Jorge Bacca  
> _Robust Illuminance Drone Detection Using Modulo Images_  
> **STSIVA 2025 Conference**, IEEE Colombia
