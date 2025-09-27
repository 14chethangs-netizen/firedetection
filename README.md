# 🔥 Fire Detection Dashboard

A **real-time fire detection system** using Python, OpenCV, Flask, and Twilio for live alerts and monitoring.

---

## Overview

This project monitors live video from a webcam and detects fire using **color-based detection** and optionally **YOLOv3 deep learning**. When fire is detected:

- The dashboard highlights the fire detection visually.
- Sends **instant SMS alerts** with location coordinates via **Twilio**.
- Shows a **live video feed continuously** (never replaced with a static image).
- Displays an **embedded Google Map** of the monitored location.
- Includes creative smoke animations for a visually appealing dashboard.

---

## Features

- Real-time fire detection using webcam
- Live video streaming via Flask
- SMS notifications with fire location
- Interactive and animated web dashboard
- Optional YOLOv3-based advanced detection
- Cross-platform (tested on Windows)

---

## Tech Stack

- **Python** – Core application logic
- **OpenCV** – Video capture and image processing
- **Flask** – Web dashboard & video streaming
- **Twilio API** – SMS notifications
- **HTML/CSS/JavaScript** – Dashboard interface

---

## Folder Structure

Fire-Detection-Dashboard/
│
├─ Fire Detection.py # Main Python application
├─ Website.html # Dashboard HTML file
├─ yolov3.weights # YOLOv3 model weights
├─ yolov3-fire.cfg # YOLOv3 configuration file
├─ CocoaExampleTests.m # Fire classes file
├─ templates/ # HTML template folder
├─ pycache/ # Python cache
└─ .venv/ # Virtual environment


---

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Fire-Detection-Dashboard.git
cd Fire-Detection-Dashboard
Create a virtual environment and activate it:

python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
Install dependencies:

pip install flask opencv-python twilio numpy
Usage
Connect your webcam.

Update Twilio credentials in Fire Detection.py.

Run the application:

python "Fire Detection.py"
Open your browser at http://localhost:5000 to view the dashboard.

How It Works
The webcam captures video frames.

Fire detection is performed using color detection (red/orange flames) and optionally YOLOv3.

When fire is detected:

The dashboard card border turns red.

Alert text appears.

SMS notifications are sent with location and video link.

The live video feed remains visible at all times; no static images replace it.

Demo

Live webcam feed with alert notification and embedded Google Maps.

License
This project is licensed under the MIT License.

Author
Chethan G S – Passionate about AI, computer vision, and IoT projects.
