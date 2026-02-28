Multi-Object Video Segmentation with SAM 2



🚀 A next-generation, prompt-driven segmentation system powered by Segment Anything Model 2 (SAM 2) for accurate multi-object image and video understanding.



🌟 Overview



This project implements an interactive multi-object segmentation and tracking system capable of:



Detecting multiple objects in images



Tracking them across video frames



Maintaining object identity and temporal consistency



Working without task-specific retraining



Unlike traditional CNN-based models that process frames independently, this system leverages transformer-based global context modeling and streaming memory to achieve smooth and stable segmentation in videos.



🔥 Why This Project Matters



Traditional segmentation systems often suffer from:



Flickering masks



Loss of object identity



Poor temporal stability



Heavy retraining requirements



By integrating SAM 2’s memory-augmented transformer architecture, this project enables reliable real-time segmentation suitable for:



📹 Surveillance systems



🤖 Autonomous systems



🎬 Video analytics



🛰️ Real-time monitoring applications



✨ Core Capabilities



✔ Prompt-based segmentation (points, bounding boxes, masks)



✔ Multi-object tracking across video frames



✔ Streaming memory for temporal consistency



✔ High-quality pixel-level mask generation



✔ No retraining required for unseen objects



✔ Near real-time performance



🧠 System Architecture



The system consists of four primary components:



🔹 Vision Transformer (ViT) Encoder



Extracts deep feature representations with global context awareness.



🔹 Prompt Encoder



Encodes user inputs (clicks, bounding boxes, masks) into embedding representations.



🔹 Streaming Memory Module



Stores object features across video frames to ensure consistent tracking.



🔹 Mask Decoder



Generates segmentation masks along with IoU confidence scores.



🛠 Technology Stack

Category	Tools Used

Language	Python 3.10+

Framework	PyTorch

Libraries	OpenCV, NumPy, Matplotlib, TorchVision

Model	SAM 2 (Pretrained)

Environment	Google Colab / Jupyter Notebook

Hardware	NVIDIA GPU (Recommended)

🚀 Getting Started

1️⃣ Clone the Repository

git clone https://github.com/your-username/your-project-name.git

cd your-project-name

2️⃣ Install Dependencies

pip install torch torchvision opencv-python numpy matplotlib

3️⃣ Download SAM 2

git clone https://github.com/facebookresearch/sam2.git

🧪 Usage

📷 Image Segmentation



Load an image



Provide a prompt (point / bounding box / mask)



Generate pixel-level segmentation masks



🎥 Video Segmentation \& Tracking



Initialize the object on the first frame using a prompt



The memory module stores object features



Objects are tracked consistently across frames



📊 Performance Highlights



🎯 Accurate object boundary detection



🔁 Strong temporal consistency



🧩 Reduced identity switching



📦 Supports multiple objects simultaneously



Input Type	Objects	Temporal Stability	Output Quality

Image	Multiple	N/A	High

Video	Multiple	High	Stable \& Smooth

📁 Project Structure

sam2/               # Core SAM 2 framework

notebooks/          # Experiment notebooks

SA\_V dataset/       # Dataset files

SAM2/               # Model integration scripts

training/           # Training / evaluation scripts

tools/              # Utility tools and outputs

README.md

requirements.txt

🏁 Conclusion



This project demonstrates how transformer-based segmentation with streaming memory overcomes the limitations of traditional models, enabling accurate, temporally consistent, and scalable multi-object video understanding.

