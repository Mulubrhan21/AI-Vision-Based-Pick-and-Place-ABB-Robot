# AI-Based Vision Pick-and-Place System for ABB Robot

## 📌 Overview
This project implements an AI-based computer vision system for automated pick-and-place
operations using an ABB industrial robot. The system detects object shape, color, position,
and orientation using a trained YOLO segmentation model and performs dynamic robotic picking.

The project was developed as part of a robotics and automation course at  
**University West (Högskolan Väst), Sweden**.

---

## 🧠 System Architecture
- Camera mounted above the workspace
- Raspberry Pi / Industrial PC running Python vision system
- AI inference using YOLO (Ultralytics)
- ArUco marker calibration for coordinate transformation
- TCP/IP socket communication
- ABB robot programmed in RAPID

---

## ⚙️ Features
- Detection of **Circle, Square, and Star**
- Color-based object filtering
- Pixel → millimeter coordinate conversion using homography
- Orientation estimation using PCA
- Graphical User Interface (GUI)
- Client–server communication with ABB robot
- Continuous pick-and-place cycles

---

## 🛠️ Technologies Used
- Python
- OpenCV
- YOLO (Ultralytics)
- Tkinter GUI
- Socket Programming (TCP/IP)
- ABB RAPID
- ArUco Markers
- Raspberry Pi / Industrial PC

---

## 📁 Project Structure
Click a folder to explore the implementation:

- 📂 **[vision_system](vision_system/)**  
  Python-based AI vision, GUI, calibration, and server communication

- 📂 **[robot_program](robot_program/)**  
  ABB RAPID program for dynamic pick-and-place

- 📂 **[model](model/)**  
  Trained YOLO segmentation model

- 📂 **[docs](docs/)**  
  Project description, course instructions, and documentation

- 📂 **[demo](demo/)**  
  Demo video and result screenshots

---

## ▶️ How to Run
1. Install dependencies  
   ```bash
   pip install -r requirements.txt
