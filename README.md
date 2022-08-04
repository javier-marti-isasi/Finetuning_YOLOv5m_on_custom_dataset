# Finetuning YOLOv5m on custom dataset
Object detection YOLOv5m finetuning on custom dataset with PyTorch. Inference on videos.

<a href="https://www.kaggle.com/datasets/mbkinaci/fruit-images-for-object-detection" target="_blank">Kaggle</a>.

https://user-images.githubusercontent.com/73080100/182164916-2c20cc3d-97a5-42da-b8de-84d156cb1d9b.mp4


Original YOLOv5 repository:
https://github.com/ultralytics/yolov5

## Directory Structure

**All the code files and folders follow the following structure.**

```
├── data.yaml
├── README.dataset.txt
├── README.roboflow.txt
├── test
│   ├── images
│   └── labels
├── train
│   ├── images
│   └── labels
└── yolov5
```

## Introduction

It is used YOLOv5m model, which has been trained on the MS COCO dataset. In the notebook provided, the model is finetuned on PASCAL VOC using PyTorch. 

YOLO is short for You Only Look Once. It is a family of single-stage deep learning based object detectors. They are capable of real-time object detection with state-of-the-art accuracy. Officially, as part of the Darknet framework, there are four versions of YOLO. Starting from YOLOv1 to YOLOv4. The Darknet framework is written in C and CUDA. YOLOv5 is the next version equivalent in the YOLO family. 

There are 5 YOLOv5 models. In this project, it is used YOLOv5m. This is the medium-sized model with 21.2 million parameters. It is perhaps the best suited model for a lot of datasets and training as it provides a good balance between speed and accuracy.

It is used the Pascal VOC 2012 Dataset dataset for training the custom YOLOv5 object detector. We can therefore detect 20 objects in images (+1 for the background class), including airplanes, bicycles, birds, boats, bottles, buses, cars, cats, chairs, cows, dining tables, dogs, horses, motorbikes, people, potted plants, sheep, sofas, trains, and tv monitors.


## Instructions

Please, follow the instruction in the provided notebook.


## Outputs

Object detection videos are saved in:
```
 yolov5/runs/detect/
 ```
