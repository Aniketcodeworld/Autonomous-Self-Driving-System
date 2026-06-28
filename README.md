#  YOLOv8 + DeepLabV3+ Fusion for Autonomous Driving Perception

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red)
![YOLOv8](https://img.shields.io/badge/YOLO-v8-green)
![DeepLabV3+-Semantic%20Segmentation-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

A computer vision project that combines **YOLOv8 Object Detection** and **DeepLabV3+ Semantic Segmentation** to improve scene understanding for autonomous driving applications.

The system detects dynamic road objects such as vehicles while simultaneously segmenting road regions, creating a richer perception pipeline suitable for intelligent transportation systems and self-driving vehicles.

---

##  Features

-  Real-time Vehicle Detection using YOLOv8
-  Semantic Road Segmentation using DeepLabV3+
-  Fusion of Detection + Segmentation Outputs
-  Confidence Score Visualization
-  Bounding Box Rendering
-  High Accuracy Detection Pipeline
-  GPU Accelerated Inference (CUDA Supported)
-  Supports Images and Videos
-  Deep Learning Based Scene Understanding

---

## Project Architecture

```
                 Input Image
                      │
        ┌─────────────┴─────────────┐
        │                           │
        ▼                           ▼
   YOLOv8 Detector            DeepLabV3+
 Object Detection       Semantic Segmentation
        │                           │
        └─────────────┬─────────────┘
                      ▼
              Feature Fusion Module
                      │
                      ▼
      Final Annotated Autonomous Scene
```

---

## Sample Output

<p align="center">
<img src="images/output.png" width="900">
</p>

The final output contains:

- Vehicle Detection
- Confidence Scores
- Bounding Boxes
- Semantic Road Segmentation
- Improved Scene Understanding

---

# Project Structure

```
YOLOv8-DeepLabV3-Fusion/
│
├── dataset/
│   ├── train/
│   ├── valid/
│   └── test/
│
├── models/
│   ├── yolov8/
│   └── deeplabv3/
│
├── notebooks/
│   ├── datasplit code.ipynb
│   ├── deeplab training code.ipynb
│   ├── deeplabv3demo.ipynb
│   ├── yolov8-testing-try.ipynb
│   └── Yolov8+deeplabV3_fusion.ipynb
│
├── outputs/
│
├── images/
│   └── output.png
│
├── requirements.txt
│
└── README.md
```

---

# Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Programming Language |
| PyTorch | Deep Learning Framework |
| YOLOv8 | Object Detection |
| DeepLabV3+ | Semantic Segmentation |
| OpenCV | Image Processing |
| NumPy | Numerical Computing |
| Matplotlib | Visualization |
| CUDA | GPU Acceleration |

---

# Dataset

The project uses datasets for:

- Vehicle Detection
- Road Scene Understanding
- Semantic Segmentation

Typical datasets include:

- Cityscapes
- BDD100K
- KITTI
- Custom Road Dataset

---

# Model Pipeline

## Step 1

Input road scene image

↓

## Step 2

YOLOv8 detects

- Cars
- Trucks
- Buses
- Motorcycles
- Persons
- Traffic Objects

↓

## Step 3

DeepLabV3+ segments

- Road
- Sidewalk
- Lane
- Background
- Vegetation
- Sky

↓

## Step 4

Fusion Algorithm combines

- Bounding Boxes
- Segmentation Mask

↓

## Step 5

Final annotated autonomous driving scene

---

# Installation

Clone the repository

```bash
git clone https://github.com/yourusername/YOLOv8-DeepLabV3-Fusion.git

cd YOLOv8-DeepLabV3-Fusion
```

Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

Windows

```bash
venv\Scripts\activate
```

Linux / Mac

```bash
source venv/bin/activate
```

Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Requirements

```
Python >= 3.10

torch

torchvision

opencv-python

numpy

matplotlib

ultralytics

Pillow

tqdm

scikit-image

scikit-learn
```

---

# Training

Train DeepLabV3+

```bash
jupyter notebook "deeplab training code.ipynb"
```

---

Train YOLOv8

```bash
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=100
```

---

# Testing

Run YOLO Detection

```bash
jupyter notebook "yolov8-testing-try.ipynb"
```

Run Segmentation Demo

```bash
jupyter notebook "deeplabv3demo.ipynb"
```

Run Fusion Model

```bash
jupyter notebook "Yolov8+deeplabV3_fusion.ipynb"
```

---

# Performance

| Model | Task |
|---------|-------------------------|
| YOLOv8 | Object Detection |
| DeepLabV3+ | Semantic Segmentation |
| Fusion Model | Scene Understanding |

The fusion approach enhances road scene perception by integrating object-level detection with pixel-level semantic information, improving robustness for autonomous driving applications.

---

# Applications

- Autonomous Vehicles
- Driver Assistance Systems (ADAS)
- Smart Transportation
- Intelligent Surveillance
- Traffic Monitoring
- Robotics
- Smart Cities
- Navigation Systems

---

# Future Improvements

- Real-time Webcam Support
- Multi-object Tracking
- Lane Detection
- Traffic Sign Recognition
- Pedestrian Tracking
- Depth Estimation
- Instance Segmentation
- TensorRT Optimization
- ONNX Deployment
- ROS Integration

---

# Author

**Aniket Mishra**

B.Tech Computer Science and Engineering

Interested in

- Artificial Intelligence
- Computer Vision
- Deep Learning
- Autonomous Systems
- Machine Learning

---

# License

This project is licensed under the MIT License.

---

# Acknowledgements

- Ultralytics YOLOv8
- PyTorch
- OpenCV
- DeepLabV3+
- Cityscapes Dataset
- KITTI Dataset

---

##  If you found this project useful, don't forget to Star the repository!
