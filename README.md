# ✋ Virtual Painter — Hand Tracking with MediaPipe & OpenCV

## 📌 Project Overview
This project implements a **virtual painter** using your webcam, where you can draw in the air using your **index finger**.  
It leverages **MediaPipe Hands** for real-time hand landmark detection and **OpenCV** for drawing on a virtual canvas.

- 👆 Draw in the air with your index finger  
- 🖼️ Live video feed + overlay canvas  
- 🎨 Switch between draw and idle mode using finger distance  
- ❌ Option to clear the canvas  
- 💾 Save your artwork  

---

## 📂 Features
- Detects **index fingertip (landmark 8)** and **thumb tip (landmark 4)**  
- If index and thumb are **far apart → Draw mode**  
- Virtual canvas overlays on the live webcam feed  
- Quit with **`q`**, clear with **`c`**, save with **`s`**  

---

## ⚙️ Installation
Clone this repository and install dependencies:

```bash
git clone https://github.com/yourusername/virtual-painter.git
cd virtual-painter

# Create virtual environment (recommended)
python -m venv .venv
# Activate (Windows)
.venv\Scripts\activate
# Activate (Mac/Linux)
source .venv/bin/activate

# Install dependencies
pip install opencv-python mediapipe numpy
