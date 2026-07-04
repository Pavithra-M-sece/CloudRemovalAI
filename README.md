# 🌤️ Generative AI-Based Cloud Removal for Satellite Images

## 📌 Project Overview

Clouds in satellite imagery often obscure important geographical information, making it difficult to perform accurate land monitoring, agriculture analysis, disaster management, urban planning, and environmental studies.

This project proposes an **AI-powered cloud removal system** that automatically detects cloud-covered regions in satellite images and reconstructs the hidden land surface using state-of-the-art Generative AI models.

The complete pipeline combines cloud segmentation, image inpainting, and image enhancement to generate visually realistic cloud-free satellite images.

---

## 🎯 Objectives

- Detect cloud-covered regions in satellite images.
- Generate cloud masks automatically.
- Remove clouds using Generative AI.
- Restore hidden land information.
- Enhance image quality after reconstruction.
- Evaluate output quality using image similarity metrics.

---

## 🚀 Proposed AI Pipeline

```
Satellite Image
       │
       ▼
Cloud Detection
(SegFormer)
       │
       ▼
Cloud Mask Generation
       │
       ▼
Cloud Removal
(LaMa Inpainting)
       │
       ▼
Image Enhancement
(Real-ESRGAN)
       │
       ▼
Cloud-Free Satellite Image
       │
       ▼
Quality Evaluation
(PSNR • SSIM)
```

---

# 📂 Project Structure

```
CloudRemovalAI/
│
├── dataset/
│   ├── raw/
│   ├── processed/
│   ├── extracted/
│   ├── metadata.csv
│   └── processed_metadata.csv
│
├── notebooks/
│   ├── Notebook1_Environment_Setup.ipynb
│   ├── Notebook2_Dataset_Preparation.ipynb
│   ├── Notebook3_Cloud_Detection.ipynb
│   ├── Notebook4_Cloud_Removal.ipynb
│   ├── Notebook5_Image_Enhancement.ipynb
│   ├── Notebook6_Evaluation.ipynb
│
├── models/
├── outputs/
├── config/
├── logs/
├── weights/
└── README.md
```

---

# 📚 Current Progress

## ✅ Completed

- Environment Setup
- Google Drive Integration
- Dataset Extraction
- Dataset Organization
- Dataset Verification
- Metadata Generation
- Dataset Visualization
- Image Preprocessing
- PyTorch Dataset Preparation
- DataLoader Pipeline

---

## 🔄 Upcoming Work

- Cloud Detection using SegFormer
- Cloud Removal using LaMa
- Image Enhancement using Real-ESRGAN
- Evaluation using PSNR & SSIM
- End-to-End Inference Pipeline
- Web Application Deployment

---

# 📊 Dataset

**Dataset Used:** RICE (Remote Sensing Image Cloud rEmoving Dataset)

The dataset contains paired:

- Cloudy Satellite Images
- Cloud-Free Ground Truth Images
- Cloud Masks

Dataset Statistics

| Category | Images |
|----------|--------|
| Cloud Images | 736 |
| Clear Images | 736 |
| Cloud Masks | 736 |

---

# 🛠️ Technology Stack

## Programming Language

- Python

## Deep Learning

- PyTorch
- TorchVision

## Computer Vision

- OpenCV
- Pillow
- NumPy

## Data Processing

- Pandas
- Scikit-learn

## Visualization

- Matplotlib

## AI Models

- SegFormer (Cloud Detection)
- LaMa (Image Inpainting)
- Real-ESRGAN (Super Resolution)

---

# 📈 Expected Results

- Accurate cloud segmentation
- High-quality cloud removal
- Enhanced satellite image reconstruction
- Improved visual clarity
- Quantitative evaluation using PSNR and SSIM

---

# 📌 Applications

- Agriculture Monitoring
- Disaster Management
- Land Cover Analysis
- Urban Planning
- Environmental Monitoring
- Forest Monitoring
- Water Resource Management
- Remote Sensing Research

---

# 📝 Evaluation Metrics

The project evaluates image quality using:

- PSNR (Peak Signal-to-Noise Ratio)
- SSIM (Structural Similarity Index)
- Visual Comparison
- Inference Time

---

# 👩‍💻 Development Environment

- Google Colab
- Jupyter Notebook
- GitHub
- Google Drive

---

# 📅 Development Roadmap

- [x] Environment Setup
- [x] Dataset Preparation
- [ ] Cloud Detection
- [ ] Cloud Removal
- [ ] Image Enhancement
- [ ] Model Evaluation
- [ ] Inference Pipeline
- [ ] Web Application
- [ ] Deployment

---

# 📜 License

This project is developed for educational and research purposes. Please refer to the original dataset and model licenses before commercial use.

---

# ⭐ Future Enhancements

- Multi-temporal cloud removal
- Transformer-based diffusion models
- Support for Sentinel-2 and Landsat datasets
- Real-time cloud removal API
- Interactive web dashboard
- Batch satellite image processing
