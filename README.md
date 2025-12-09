# YOLOv8 Object Detection Using Webcam

This project implements **real-time object detection using the YOLOv8 Nano model** with a webcam feed.  
It is optimized for **CPU-based systems**, making it suitable for laptops and educational environments without requiring GPU acceleration.

---

## 🚀 Key Features

### ✅ Model Loading
- Uses **YOLOv8 Nano (`yolov8n.pt`)**  
- Fastest YOLOv8 variant ideal for CPU inference

---

### ✅ Real-time Webcam Detection
Provides continuous object detection with:

- 📦 **Bounding boxes** around detected objects  
- 🎯 **Confidence scores** for predictions  
- ⏱️ **FPS counter** and runtime statistics  
- ⚙️ **Configurable duration** for detection  
- 🎚️ **Adjustable confidence threshold** to filter weak detections

---

### ✅ Static Image Detection
Includes an optional function to:

- Run object detection on static image files
- Quickly test detection quality without webcam usage

---

### ✅ Performance Monitoring

The system tracks and displays:

- Frames Per Second (**FPS**)  
- Total processed frames  
- Detection time statistics

These metrics help evaluate model efficiency on CPU hardware.

---

### ✅ Model Information Display

Lists and prints:

- All supported **detectable object classes**
- Model configuration details

---

---

## 🛠️ How to Use This Notebook

1. Open **Jupyter Notebook** or **VS Code Notebook environment**
2. Copy all cells from the project notebook into a notebook file
3. Run cells **sequentially from top to bottom**

---

### ▶️ Start Webcam Detection

- **Cell 6** starts webcam detection for **30 seconds**
- Press **`Q`** anytime to quit early

After execution, the webcam feed will appear with live object detection overlay.

---

---

## ⚙️ CPU Optimization Notes

This notebook is optimized for systems without GPUs:

- ✅ **YOLOv8 Nano (`yolov8n`)** selected for fastest CPU inference
- ✅ **Frame size:** `640 x 480`  
  - Balances detection accuracy and processing speed
- ✅ **Confidence threshold:** `0.5`  
  - Filters weak detections and improves display clarity
- ✅ **CPU device enforced:**  
  ```python
  device = 0   # Forces CPU usage

