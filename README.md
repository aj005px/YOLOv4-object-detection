# yolov4-object-detection

Real-time object detection using YOLOv4 and Darknet, built and tested on Google Colab with GPU support.

## Overview

This project uses [YOLOv4](https://github.com/AlexeyAB/darknet) — one of the most powerful and accurate real-time object detection models — to detect objects in custom images. The entire setup runs on Google Colab, making it easy to use without any local installation.

## Features

- YOLOv4 object detection using the Darknet framework
- GPU + CUDNN acceleration for fast inference
- Tested on the COCO dataset (80 object classes)
- Supports custom image uploads via Google Colab

## Requirements

- Google Colab (with GPU runtime enabled)
- No local setup needed — everything runs in the notebook

## Getting Started

1. Open the notebook in Google Colab
2. Set the runtime to **GPU** (`Runtime > Change runtime type > GPU`)
3. Run all cells in order
4. Upload your own image when prompted to test detection

## How It Works

1. Clones the Darknet repository and compiles it with GPU/CUDNN/OpenCV support
2. Downloads the pre-trained `yolov4.weights` file
3. Runs detection on a sample image (`dog.jpg`) from the Darknet dataset
4. Accepts a custom image upload and runs detection on it
5. Displays the output with bounding boxes and labels

## Example Output

After running detection, a `predictions.jpg` file is generated showing detected objects with bounding boxes and confidence scores.

## References

- [Darknet / YOLOv4 by AlexeyAB](https://github.com/AlexeyAB/darknet)
- [YOLOv4 Paper](https://arxiv.org/abs/2004.10934)
- [COCO Dataset](https://cocodataset.org/)
