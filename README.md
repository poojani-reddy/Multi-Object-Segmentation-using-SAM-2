Multi-Object Video Segmentation with SAM 2

✨ A next-generation prompt-driven segmentation system powered by Segment Anything Model 2 (SAM 2) for accurate multi-object image and video understanding.

🌟 Project Overview

This project builds an interactive multi-object segmentation and tracking system capable of:

🔍 Detecting multiple objects in images

🎥 Tracking objects across video frames

🔁 Maintaining object identity & temporal consistency

🚫 Operating without task-specific retraining

Unlike traditional CNN-based models that process frames independently, this system leverages:

🧠 Transformer-based global context modeling

💾 Streaming memory for long-term video consistency

✅ Result: Smooth, stable, high-quality segmentation across frames

🔥 Why This Project Matters

Traditional segmentation systems often suffer from:

❌ Flickering masks

❌ Identity switching

❌ Poor temporal stability

❌ Heavy retraining requirements

By integrating SAM 2’s memory-augmented transformer architecture, this project enables reliable segmentation for:

📹 Surveillance Systems

🤖 Autonomous Vehicles & Robotics

🎬 Video Analytics

🛰️ Real-Time Monitoring Applications

✨ Core Features

✔ Prompt-based segmentation (points, bounding boxes, masks)
✔ Multi-object tracking across video frames
✔ Streaming memory for temporal stability
✔ High-quality pixel-level mask generation
✔ No retraining for unseen objects
✔ Near real-time performance

🧠 System Architecture

The system consists of four major components:

🔹 1. Vision Transformer (ViT) Encoder

Extracts deep feature representations with global contextual awareness.

🔹 2. Prompt Encoder

Encodes user inputs (clicks, bounding boxes, masks) into embedding vectors.

🔹 3. Streaming Memory Module

Stores object-level features across frames to maintain identity consistency.

🔹 4. Mask Decoder

Generates segmentation masks with IoU confidence scores.

🛠 Technology Stack
Category	Tools
🐍 Language	Python 3.10+
🔥 Framework	PyTorch
📚 Libraries	OpenCV, NumPy, Matplotlib, TorchVision
🤖 Model	SAM 2 (Pretrained)
💻 Environment	Google Colab / Jupyter
⚡ Hardware	NVIDIA GPU (Recommended)
🚀 Getting Started
1️⃣ Clone Repository
git clone https://github.com/your-username/your-project-name.git
cd your-project-name
2️⃣ Install Dependencies
pip install torch torchvision opencv-python numpy matplotlib
3️⃣ Download SAM 2
git clone https://github.com/facebookresearch/sam2.git
🧪 Usage Guide
📷 Image Segmentation

Load an image

Provide a prompt (point / box / mask)

Generate pixel-level segmentation masks

🎥 Video Segmentation & Tracking

Initialize object in first frame

Memory module stores object features

Objects are tracked consistently across frames

📊 Performance Highlights

🎯 Precise object boundary detection

🔁 Strong temporal consistency

🧩 Reduced identity switching

📦 Supports multiple objects simultaneously

Input	Objects	Temporal Stability	Output
Image	Multiple	N/A	High Quality
Video	Multiple	High	Stable & Smooth
📁 Project Structure
sam2/               # Core SAM 2 framework
notebooks/          # Experiment notebooks
SA_V_dataset/       # Dataset files
integration/        # Model integration scripts
training/           # Training & evaluation
tools/              # Utilities
README.md
requirements.txt
🏁 Conclusion

This project demonstrates how transformer-based segmentation with streaming memory overcomes traditional limitations by enabling:

✅ Accurate segmentation

✅ Temporal consistency

✅ Scalable multi-object tracking

✅ Near real-time performance
