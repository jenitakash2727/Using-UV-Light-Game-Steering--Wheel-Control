# Using-UV-Light-Game-Steering--Wheel-Control
Control a virtual car using hand gestures with OpenCV and Python.”  “Real-time hand gesture detection for steering using HSV color tracking.”

Real-time hand gesture-based UV steering control using OpenCV and Python.

📦 requirements.txt
numpy>=1.24.0
opencv-python>=4.8.0
imutils>=0.5.4


⚠️ directkeys.py should be included in the project folder manually. It’s used for simulating key presses in Windows.

README.md
# 🎮 UV Steering Hand Gesture Control

![Python](https://img.shields.io/badge/Python-3.x-blue)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

Control a virtual car in real-time using hand gestures detected through your webcam.  
This project uses OpenCV and Python to detect a colored object and simulate LEFT (`A`) and RIGHT (`D`) key presses.

---

## ✨ Features
- 🖐 Real-time hand gesture detection using HSV color tracking
- ⬅️➡️ Control LEFT (`A`) and RIGHT (`D`) movements
- 👁️ Visual guidance with rectangles and labels on the webcam feed
- ⚡ Adjustable color detection for different objects
- 🎨 Dark-themed webcam overlay for clear control zones

---

## 🛠️ Tech Stack
- Python 3.x
- OpenCV (Computer Vision)
- NumPy (Numerical computations)
- imutils (Image/video utilities)
- directkeys.py (Keyboard simulation for Windows)

---

## 📂 Project Structure


├── uv_steering.py # Main application code
├── directkeys.py # Keyboard control module
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── demo_image.gif # Optional demo screenshot/GIF


---

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/UV-Steering-Hand-Gesture-Control.git
cd UV-Steering-Hand-Gesture-Control


Create a virtual environment and activate it:

# Mac/Linux
python -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate


Install dependencies:

pip install -r requirements.txt


Ensure directkeys.py is present in the folder.

▶️ Usage

Run the main script:

python uv_steering.py


Use a colored object (matching HSV values in code) to control steering.

Move the object left or right in the top half of the webcam to simulate A or D key presses.

Press q to quit the application.

🎨 HSV Color Adjustment

Modify the following in uv_steering.py to match your object:

colourLower = np.array([125, 50, 50])
colourUpper = np.array([150, 255, 255])

🖼 Demo

<!-- Replace with actual GIF/screenshot -->

🔧 Future Enhancements

Add support for multiple objects and gestures

Implement smoother steering using trajectory prediction

Cross-platform support (Linux/macOS)

Add custom UI overlay for feedback

🤝 Contributing

Contributions are welcome!

Fork this repository

Create your feature branch (git checkout -b feature-name)

Commit your changes (git commit -m "Add feature")

Push to the branch (git push origin feature-name)

Open a Pull Request

📜 License

This project is licensed under the MIT License. See LICENSE
 for details.

🙌 Acknowledgements

OpenCV for computer vision

NumPy for numerical operations

imutils for video utilities

directkeys.py for keyboard simulation
