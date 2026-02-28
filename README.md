<div align="center">

# 🚀 Multi-Object Video Segmentation using SAM 2

### 🧠 Transformer-Based • 💾 Memory-Augmented • 🎯 Prompt-Driven • ⚡ Real-Time

<br>

<img src="https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python"/>
<img src="https://img.shields.io/badge/PyTorch-DeepLearning-red?style=flat-square&logo=pytorch"/>
<img src="https://img.shields.io/badge/Model-SAM2-green?style=flat-square"/>
<img src="https://img.shields.io/badge/GPU-NVIDIA-orange?style=flat-square&logo=nvidia"/>

</div>

---

## 📌 Project Overview

> An interactive **multi-object segmentation and tracking system** powered by **Segment Anything Model 2 (SAM 2)**.

This project enables:

| Capability | Description |
|------------|------------|
| 🔍 Multi-Object Detection | Detect multiple objects in images |
| 🎥 Video Tracking | Track objects consistently across frames |
| 🔁 Temporal Stability | Maintain object identity using memory |
| 🚫 Zero Retraining | Works on unseen objects without retraining |

---

## ❗ Problems with Traditional Models

Traditional CNN-based segmentation systems suffer from:

- ❌ Flickering masks  
- ❌ Identity switching  
- ❌ Frame-by-frame inconsistency  
- ❌ Heavy retraining requirements  

---

## ✅ How This Project Solves It

| Traditional Approach | Our Approach |
|----------------------|--------------|
| Frame-by-frame processing | Transformer-based global modeling |
| No temporal memory | Streaming memory module |
| Frequent identity loss | Persistent object embeddings |
| Task-specific training | Prompt-driven zero-shot segmentation |

---

## 🧠 System Architecture

```
Input Frame + Prompt
        ↓
Vision Transformer Encoder
        ↓
Prompt Encoder
        ↓
Streaming Memory Module
        ↓
Mask Decoder
        ↓
Segmentation Mask + IoU Score
```

### 🔹 Architecture Components

| Component | Role |
|-----------|------|
| **Vision Transformer (ViT)** | Extracts global contextual features |
| **Prompt Encoder** | Converts clicks/boxes into embeddings |
| **Streaming Memory** | Maintains cross-frame object identity |
| **Mask Decoder** | Generates high-quality pixel masks |

---

## 🎯 Core Features

- ✔ Prompt-based segmentation (points, boxes, masks)
- ✔ Multi-object tracking across videos
- ✔ High-quality pixel-level masks
- ✔ Strong temporal consistency
- ✔ Near real-time inference
- ✔ No retraining required

---

## 🛠 Tech Stack

| Category | Technology |
|----------|------------|
| 🐍 Language | Python 3.10+ |
| 🔥 Framework | PyTorch |
| 🤖 Model | SAM 2 (Pretrained) |
| 📚 Libraries | OpenCV, NumPy, Matplotlib |
| 💻 Environment | Google Colab / Jupyter |
| ⚡ Hardware | NVIDIA GPU Recommended |

---

## 🚀 Installation

### 1️⃣ Clone Repository
```bash
git clone https://github.com/your-username/your-project-name.git
cd your-project-name
```

### 2️⃣ Install Dependencies
```bash
pip install torch torchvision opencv-python numpy matplotlib
```

### 3️⃣ Download SAM 2
```bash
git clone https://github.com/facebookresearch/sam2.git
```

---

## 🧪 Usage

### 📷 Image Segmentation
1. Load image  
2. Provide prompt (point / box / mask)  
3. Generate segmentation mask  

### 🎥 Video Segmentation
1. Initialize object in first frame  
2. Memory stores object features  
3. Objects tracked across frames  

---

## 📊 Performance Summary

| Input Type | Multi-Object | Temporal Stability | Output Quality |
|------------|-------------|-------------------|----------------|
| Image | ✅ Yes | N/A | High |
| Video | ✅ Yes | High | Stable & Smooth |

---

## 📂 Project Structure

```
sam2/               # Core SAM2 framework
notebooks/          # Experiments
dataset/            # Dataset files
integration/        # Model integration
training/           # Evaluation scripts
tools/              # Utilities
README.md
requirements.txt
```

---

## 🏁 Conclusion

This project demonstrates how **Transformer-based segmentation with streaming memory** overcomes traditional video segmentation limitations.

### 🚀 Enables:
- 🎯 Accurate object boundaries  
- 🔁 Strong temporal consistency  
- 📦 Scalable multi-object tracking  
- ⚡ Near real-time performance  

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star!

</div>
