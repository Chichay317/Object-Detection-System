# Object-Detection-System

This is a real-time object detection system that identifies and labels multiple objects in images or videos using a pre-trained SSD MobileNet model. 
It applies bounding boxes, confidence scoring, and label visualization for clear detection results.

Features
1. Loads and uses a pre-trained ssd_mobilenet_v3_large_coco model for object detection
2. Reads class labels from a Labels.txt file (COCO dataset classes)
3. Detects objects in images or videos and draws bounding boxes with labels and confidence
4. Handles overlapping labels with dynamic offsets and filled backgrounds for readability
5. Supports webcam input for live object detection
6. Adjustable confidence threshold to control detection sensitivity
7. Compatible with large images and video frames with scaling for visualization

How it Works
1. The model is loaded with its frozen graph and configuration file
2. Class labels are read from a text file (Labels.txt) corresponding to COCO classes
3. For each input image or video frame:
a) Objects are detected with bounding boxes and confidence scores

b) Bounding boxes are drawn around detected objects

c) Labels are placed dynamically above boxes with a filled rectangle background to prevent overlapping

4. The processed image or video frame is displayed in real time

5. For videos, detection runs frame by frame and updates continuously, supporting live camera input

6. The confidence threshold can be adjusted to include more or fewer detections
