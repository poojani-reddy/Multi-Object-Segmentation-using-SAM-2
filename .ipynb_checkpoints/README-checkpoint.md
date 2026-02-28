Multi-Object Video Segmentation using SAM 2

An interactive, transformer-based system for multi-object image and video segmentation using SAM 2 (Segment Anything Model 2).
This project enables prompt-based segmentation, memory-driven video tracking, and temporally consistent multi-object segmentation without retraining.

📌 Project Overview

Traditional segmentation models process video frames independently, leading to:

Flickering masks

Loss of object identity

Poor temporal consistency

This project overcomes those limitations by leveraging SAM 2, a transformer-based segmentation framework with streaming memory, enabling accurate and stable segmentation across images and videos.

✨ Key Features

✅ Pixel-level multi-object segmentation

🎯 Prompt-based interaction (points, bounding boxes, masks)

🎥 Video object tracking with memory

🔁 Temporal consistency across frames

⚡ Near real-time performance

🚫 No retraining required

🧠 Transformer-based global context modeling

🧠 System Architecture
Core Components

Vision Transformer (ViT) Encoder – Extracts image features

Prompt Encoder – Encodes user inputs

Memory Module – Stores object features across video frames

Mask Decoder – Generates segmentation masks and IoU scores

🛠️ Tech Stack
Category	Tools
Language	Python 3.10+
Framework	PyTorch
Libraries	NumPy, OpenCV, Matplotlib, TorchVision
Model	SAM 2 (Pretrained)
Environment	Google Colab / Jupyter Notebook
Hardware	NVIDIA GPU (Recommended)

🚀 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/your-project-name.git
cd your-project-name
2️⃣ Install Dependencies
pip install torch torchvision opencv-python numpy matplotlib
3️⃣ Download SAM 2
git clone https://github.com/facebookresearch/sam2.git

🧪 Usage
Image Segmentation

Provide an image

Add prompt (click / bounding box / mask)

Generate pixel-level segmentation

Video Segmentation & Tracking

Initialize object with prompt on first frame

Track objects across frames using memory


📊 Results

🔹 Accurate object boundaries

🔹 Stable segmentation across frames

🔹 Reduced identity switching

🔹 Supports multiple objects simultaneously

Input	Objects	 Temporal Stability	  Output Quality
Image	Multiple 	    N/A	               High
Video	Multiple    	High	       Stable Masks


🔗 Project Demo Video:
https://drive.google.com/your-video-link


📁 Project Structure
├── sam2/
├── notebooks/
├── input_videos/
├── outputs/
├── README.md
└── requirements.txt