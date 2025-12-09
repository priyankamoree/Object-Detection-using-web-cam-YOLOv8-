# Key Features:

Model Loading - Loads YOLOv8 nano (fastest for CPU)
Real-time Webcam Detection - Continuous object detection with:

Bounding boxes and confidence scores
FPS counter and statistics
Configurable duration and confidence threshold

Static Image Detection - Optional function to test on images
Performance Monitoring - Tracks FPS and processing metrics
Model Information - Displays all detectable classes

# To use this notebook:

Copy the cells into a Jupyter notebook
Run cells sequentially from top to bottom
Cell 6 starts the webcam detection for 30 seconds (press 'q' to quit early)

# Important notes for CPU optimization:

The nano model (yolov8n) is fastest for CPU processing
Frame size is set to 640x480 for good balance between speed and accuracy
Confidence threshold at 0.5 filters out weak detections
Processing happens on CPU device (device=0 forces CPU)

# Customization options in the notebook:

Change detection duration: detect_objects_webcam(duration=60)
Adjust confidence threshold: conf_threshold=0.7
Switch to faster model: YOLO('yolov8s.pt') in Cell 3
Reduce frame size for faster FPS in Cell 5
