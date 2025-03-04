# Pothole-Detection-Using-YOLO

📌 Overview
This project detects potholes in images and videos using YOLOv8. The goal is to assist in road maintenance and accident prevention by providing an efficient method for pothole detection.

🛠️ Workflow
This project follows a structured approach for training and detection:

Data Annotation with Roboflow

Uploaded videos/images to Roboflow.
Segmented potholes by drawing outlines.
Exported the labeled dataset for training.
Model Training

Used the YOLOv8 model for object detection & segmentation.
Trained on the annotated dataset using Ultralytics YOLO.
Generated a best_advanced.pt model file after training.
Integration & Detection

Loaded the trained model into Python using the Ultralytics YOLO library.
Processed images/videos to detect potholes with bounding boxes & segmentation masks.
Displayed the results using OpenCV.
📁 Dataset
Created using Roboflow with manually segmented pothole images.
Contains multiple road conditions for better model generalization.
Includes bounding boxes & segmentation masks for precise detection.

🔍 Model Details
Architecture: YOLOv8
Dataset: Custom pothole dataset from Roboflow
Pretrained Weights: best_advanced.pt
Framework: Ultralytics YOLO

📝 Future Improvements
Increase dataset size for better accuracy.
Deploy as a web or mobile application.
Integrate with IoT devices for real-time road monitoring.
