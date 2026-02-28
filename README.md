<div align="center">
🚀 Multi-Object Video Segmentation with SAM 2
Prompt-Driven • Transformer-Based • Memory-Augmented • Real-Time
<img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/PyTorch-Deep%20Learning-red?style=for-the-badge&logo=pytorch" /> <img src="https://img.shields.io/badge/Model-SAM2-green?style=for-the-badge" /> <img src="https://img.shields.io/badge/GPU-Recommended-orange?style=for-the-badge&logo=nvidia" /> </div>
✨ Overview

This project implements an interactive multi-object segmentation and tracking system powered by Segment Anything Model 2 (SAM 2).

It enables:

🔍 Accurate multi-object image segmentation

🎥 Stable tracking across video frames

🔁 Temporal consistency with streaming memory

🚫 Zero retraining for unseen objects

Unlike traditional CNN-based models, this system uses:

🧠 Transformer-based global feature modeling

💾 Streaming memory for cross-frame consistency

Result: Smooth, stable, high-quality segmentation in images and videos

🔥 Why This Project Stands Out

Traditional segmentation models suffer from:

❌ Flickering masks

❌ Identity switching

❌ Frame-by-frame inconsistency

❌ Heavy retraining needs

This project solves those using memory-augmented transformer architecture, making it suitable for:

📹 Surveillance Systems

🤖 Autonomous Systems

🎬 Video Analytics

🛰️ Real-Time Monitoring

🧠 System Architecture
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
Segmentation Masks + IoU Score
🔹 Vision Transformer (ViT)

Extracts deep global contextual features.

🔹 Prompt Encoder

Converts clicks, boxes, or masks into embeddings.

🔹 Streaming Memory

Stores object features across frames for identity preservation.

🔹 Mask Decoder

Generates pixel-level masks with confidence scores.

🎯 Core Features

✔ Prompt-based segmentation

✔ Multi-object tracking

✔ Streaming memory consistency

✔ High-quality mask generation

✔ Works on unseen objects

✔ Near real-time inference

🛠 Tech Stack
Category	Technology
Language	Python 3.10+
Framework	PyTorch
Model	SAM 2 (Pretrained)
Libraries	OpenCV, NumPy, Matplotlib
Environment	Colab / Jupyter
Hardware	NVIDIA GPU
🚀 Installation
git clone https://github.com/your-username/your-project-name.git
cd your-project-name
pip install -r requirements.txt

Download SAM 2:

git clone https://github.com/facebookresearch/sam2.git
🧪 Usage
📷 Image Segmentation

Load image

Provide prompt (point / box / mask)

Generate segmentation mask

🎥 Video Segmentation

Initialize object in first frame

Memory module stores features

Objects tracked across frames

📊 Performance
Input	Multi-Object	Temporal Stability	Output Quality
Image	✅	N/A	High
Video	✅	High	Stable & Smooth
📂 Project Structure
sam2/               # Core framework
notebooks/          # Experiments
dataset/            # Data
integration/        # Model integration
training/           # Evaluation scripts
tools/              # Utilities
🏁 Conclusion

This project demonstrates how transformer-based segmentation with streaming memory overcomes traditional video segmentation limitations, enabling:

🎯 Accurate object boundaries

🔁 Strong temporal consistency

📦 Multi-object scalability

⚡ Real-time capable performance
