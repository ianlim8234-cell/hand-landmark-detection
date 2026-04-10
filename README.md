# Hand Landmark Detection (MediaPipe + OpenCV)

## Overview

This project uses MediaPipe and OpenCV to detect and visualize hand landmarks in real time using your webcam. It supports detecting up to two hands and draws key points (and optionally connections) on each hand.

If your goal is just visualization, this is all you need—no machine learning model required.

---

## Features

* Real-time hand tracking
* Supports up to 2 hands
* 21 landmarks per hand
* Lightweight and fast

---

## Demo

Shows:

* Webcam feed
* Green dots on each joint of your hand

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/hand-landmark-detection.git
cd hand-landmark-detection
```

### 2. Install dependencies

```bash
pip install opencv-python mediapipe numpy
```

---

## Usage

Run the script:

```bash
python main.py
```

Press `ESC` to exit.

---

## Common Issues

### iPhone camera is being used instead of MacBook camera

macOS may automatically switch to your iPhone via Continuity Camera.

Fix:

* Disable Continuity Camera in system settings
* Or change camera index in OpenCV:

```python
cap = cv2.VideoCapture(1)
```

---

## Project Structure

```
hand-landmark-detection/
│
├── main.py
├── hand_landmarker.task
├── README.md
```
