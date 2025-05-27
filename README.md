# 🚗 Car Counter using YOLOv8 and OpenCV

A real-time car counting system using **YOLOv8**, **OpenCV**, and **cvzone**. The program detects and tracks vehicles in a video stream and classifies them as **incoming** or **outgoing** based on slanted virtual lines. The live count is displayed on screen. Optimized for CPU usage.

## 🔍 Features

- Real-time car detection with YOLOv8n
- Unique ID tracking for each vehicle
- Slanted line-based direction detection
- Incoming/outgoing vehicle count display
- CPU-only execution (no GPU required)

## 📽️ How It Works

- The video is divided into left (outgoing) and right (incoming) zones.
- Slanted lines are drawn to define entry/exit directions.
- Cars are detected and assigned tracking IDs.
- When a car crosses a line in the right direction, it is counted once.
- Counts are shown on the video frame.

## 📁 Project Structure

project/
├── videos/
│ └── expway.mp4 # Input video file
├── .venv/yolo-Weight/
│ └── yolov8n.pt # YOLOv8n model weights
└── main.py # Main Python script

perl
Copy
Edit

## 🛠️ Requirements

Install the dependencies:

```bash
pip install ultralytics opencv-python cvzone torch
▶️ Run the Script
bash
Copy
Edit
python main.py
Press q to quit the video window.

📦 Model
YOLOv8n (yolov8n.pt)

From Ultralytics YOLOv8

📄 License
This project is for educational and research purposes only.

