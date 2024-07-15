## Day 2 YOLO Command Line Interface (CLI) Guide

Welcome to the YOLO Command Line Interface (CLI) guide. This document will help you understand how to use the YOLO CLI commands to perform various tasks such as segmentation, classification, and detection using different modes and models.

### Overview
We will cover the following tasks using the YOLO CLI:
1. Segmentation
2. Classification
3. Detection

Each task can be performed in three different modes:
- Predict
- Validate (val)
- Train

### Models
We will use the following models for each task:
1. **Detection**: `yolov8n.pt`
2. **Segmentation**: `yolov8n-seg`
3. **Classification**: `yolov8n-cls`

### Commands

#### 1. Segmentation

##### Predict Mode
To perform segmentation prediction:
```sh
yolo mode=predict task=segment model="yolov8n-seg" source="path/to/images"
```

##### Validation Mode
To perform segmentation validation:
```sh
yolo mode=val task=segment model="yolov8n-seg" source="path/to/images"
```

##### Train Mode
To train a segmentation model:
```sh
yolo mode=train task=segment model="yolov8n-seg" source="path/to/images"
```

#### 2. Classification

##### Predict Mode
To perform classification prediction:
```sh
yolo mode=predict task=classify model="yolov8n-cls" source="path/to/images"
```

##### Validation Mode
To perform classification validation:
```sh
yolo mode=val task=classify model="yolov8n-cls" source="path/to/images"
```

##### Train Mode
To train a classification model:
```sh
yolo mode=train task=classify model="yolov8n-cls" source="path/to/images"
```

#### 3. Detection

##### Predict Mode
To perform detection prediction:
```sh
yolo mode=predict task=detect model="yolov8n.pt" source="path/to/images"
```

##### Validation Mode
To perform detection validation:
```sh
yolo mode=val task=detect model="yolov8n.pt" source="path/to/images"
```

##### Train Mode
To train a detection model:
```sh
yolo mode=train task=detect model="yolov8n.pt" source="path/to/images"
```

### Notes
- Replace `"path/to/images"` with the actual path to your image file or directory.
- Ensure the model files (`yolov8n.pt`, `yolov8n-seg`, `yolov8n-cls`) are in the correct location or provide the absolute path to these model files.

### Example
For example, if you want to predict segmentation on images located in the `images` directory:
```sh
yolo mode=predict task=segment model="yolov8n-seg" source="images"
```

By following the commands provided in this guide, you should be able to perform segmentation, classification, and detection tasks using the YOLO CLI effectively. If you encounter any issues, refer to the YOLO documentation or seek assistance from the community.

---

This README file serves as a quick reference to help you utilize the YOLO CLI for various tasks efficiently. Happy experimenting with YOLO!
