# AgriScan: Offline-First Plant Disease Detection 🌱

![Status](https://img.shields.io/badge/Status-In%20Development-yellow) ![Python](https://img.shields.io/badge/Python-3.10-blue) ![Edge AI](https://img.shields.io/badge/Edge-ONNX-green)

AgriScan is an edge-computing solution designed to detect plant diseases (Potato Early/Late Blight) on low-end Android devices without internet connectivity.

## 🏗️ Architecture (In Progress)
The system follows a hybrid edge-cloud architecture:
1.  **Training:** ResNet18/MobileNetV3 trained on PyTorch.
2.  **Optimization:** FP32 models converted to **INT8** via ONNX Runtime for 4x compression.
3.  **Inference:** Running locally on CPU (Android/WebAssembly).

## 🛠️ Tech Stack
* **Core:** PyTorch, OpenCV
* **Edge Inference:** ONNX Runtime
* **Backend:** FastAPI (Model Registry)
* **Deployment:** Docker

## 🚀 Roadmap
- [x] Train baseline ResNet models for Potato/Chicken disease.
- [ ] Implement ONNX Quantization pipeline.
- [ ] Build FastAPI backend for model versioning.
- [ ] Deploy client-side inference (Next.js/PWA).

---
*Note: This repository is currently under active development. Some modules are being migrated from local research notebooks.*
