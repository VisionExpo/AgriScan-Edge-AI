# AgriScan: Edge AI Disease Detection System 🌿📱

![Status](https://img.shields.io/badge/Status-Research%20Prototype-orange) ![Focus](https://img.shields.io/badge/Focus-Edge%20Computing-blue) ![Model](https://img.shields.io/badge/Model-MobileNet%20%7C%20ONNX-green)

> **⚠️ Project Status:** This repository is the clean implementation of the AgriScan research. It is currently being populated with the V2 codebase, moving from cloud-based VGG16 models to offline-first MobileNetV3 architectures optimized for Android.

## 📋 The Problem
Farmers in rural India lack internet connectivity. Cloud-based AI APIs fail in these regions. AgriScan solves this by moving the inference **to the edge** (On-Device).

## 🏗️ Architecture
1.  **Training:** PyTorch (ResNet/MobileNet)
2.  **Optimization:** ONNX Quantization (FP32 -> INT8)
3.  **Inference:** ONNX Runtime (CPU)

## 📂 Repository Structure
* `/models` - Optimized ONNX model weights.
* `/notebooks` - Research and training experiments.
* `/src` - FastAPI backend for model registry.

## 🚀 Roadmap
- [x] Train baseline models for Poultry/Potato disease.
- [ ] Implement quantization pipeline.
- [ ] Deploy offline PWA.
