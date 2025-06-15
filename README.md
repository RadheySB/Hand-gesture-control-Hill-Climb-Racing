🖐️ Hand Gesture Control for Hill Climb Racing 🚗

A Python project that lets you control Hill Climb Racing using just your hand gestures via a webcam! Built using MediaPipe and OpenCV, the system detects hand gestures in real-time and maps them to accelerator and brake keyboard inputs.

✊ Fist → Brake

✋ Open palm (5 fingers) → Accelerate

Ideal for hands-free, fun interaction with simple racing games on Windows.

🛠️ Features

Real-time hand detection and gesture recognition

Maps gestures to keyboard inputs using directkeys.py

Compatible with any keyboard-driven racing game

📦 Requirements

Python 3.7+

opencv-python

mediapipe

A webcam

directkeys.py (included in this repo)

Install dependencies

pip install opencv-python mediapipe

🚀 Getting Started
Clone the repository

bash
Copy
Edit
git clone https://github.com/RadheySB/Hand-gesture-control-Hill-Climb-Racing.git
cd Hand-gesture-control-Hill-Climb-Racing
Run the script

bash
Copy
Edit
python hand_gesture_vehicle_control.py
Control the game

🖐️ Show an open palm (all fingers) to accelerate

✊ Close your fist to brake

✋ Any other gesture stops input

Exit the script by pressing q

📁 Project Structure
bash
Copy
Edit
Hand-gesture-control-Hill-Climb-Racing/
├── hand_gesture_vehicle_control.py   # Main script
├── directkeys.py                     # Custom keypress module
└── README.md
⚙️ How It Works
Uses mediapipe to detect hand landmarks.

Calculates finger states by comparing landmark positions.

If:

All 5 fingers are detected → sends accelerator key press.

No fingers (fist) → sends brake key press.

Keys are simulated using ctypes via directkeys.py.

⚠️ Notes
Works only on Windows due to directkeys implementation.

Ensure proper lighting for accurate hand detection.

Designed for use with games that accept keyboard input.

