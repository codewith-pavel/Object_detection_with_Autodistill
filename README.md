# Real-Time Fire Detection with Drones and Edge Computing

This repository contains the implementation of a real-time fire detection system integrating lightweight deep learning models, drones, and edge computing. The system leverages YOLOv8, DETR, and knowledge distillation techniques for efficient fire detection in resource-constrained environments.

## 📖 Abstract
Fire accidents pose significant threats to life, property, and the environment. This project addresses the challenge by deploying a drone-based system with edge computing for real-time fire detection. Key contributions include:
- A **comprehensive dataset** of 7,187 fire images.
- **Knowledge distillation** from YOLOv8m (teacher) to YOLOv8n (student), achieving **95.21% accuracy**.
- A **custom-built drone** with Raspberry Pi 5 and Pi Camera for live inference at **8 FPS**.

## ✨ Features
- **Dataset**: Combined public datasets with augmented fire/no-fire images.
- **Models**: YOLOv8, DETR, Detectron2, and Autodistill-based knowledge distillation.
- **Hardware**: DJI F450 drone, Raspberry Pi 5, Pi Camera, and Pixhawk flight controller.
- **Real-Time Deployment**: Lightweight YOLOv8n model optimized for edge devices.

## 📁 Dataset
The dataset comprises 7,187 images across categories like forest fires, vehicle fires, and drone-view fires.

**Preprocessing steps:**

- **Augmentation**: Horizontal/vertical flips, saturation adjustments, noise addition.
- **Splitting**: 80% training, 10% validation, 10% testing.

## 📊 Results

| Model               | Accuracy | F1 Score | mAP@50 | Frame Rate (FPS) |
|---------------------|----------|----------|--------|------------------|
| YOLOv8n (Distilled) | 95.21%   | 0.985    | 93.31% | 8                |
| DETR (Distilled)    | 81.10%   | 0.806    | 71.40% | 3                |

## 📜 Citation
If you use this work, please cite the original paper:

```bibtex
@article{titu2024real,
  title={Real-Time Fire Detection: Integrating Lightweight Deep Learning Models on Drones with Edge Computing},
  author={Titu, Md Fahim Shahoriar and others},
  journal={Drones},
  volume={8},
  pages={483},
  year={2024},
  doi={https://doi.org/10.3390/drones8090483}
}
```
