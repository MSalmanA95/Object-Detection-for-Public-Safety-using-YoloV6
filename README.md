# Object-Detection-for-Public-Safety-using-YoloV6
Advanced Weapon Detection System: This repository houses the YOLOv6-based object detection system designed to enhance security by identifying concealed weapons in x-ray images. The system features real-time alerts, high accuracy, easy scalability, and user-friendly operation, making it an essential tool for security personnel in various settings.

This repository contains the implementation of an advanced weapon detection system that utilizes the YOLOv6 object detection model to identify concealed weapons such as guns, knives, and shurikens in x-ray images. The system is designed to enhance security measures by providing real-time alerts to security personnel.

## Features

- Weapon Detection: Detects various types of concealed weapons within x-ray images using the YOLOv6 model.
- Real-Time Alerts: Configures real-time notifications for security personnel upon detection of a potential threat.
- High Accuracy and Performance: Utilizes the optimized YOLOv6 model for high precision and performance in weapon detection.
- User-Friendly: Designed for easy integration and use in existing security systems.

## Installation
 ```
1. Clone the Repository:
   ```
!git clone https://github.com/meituan/YOLOv6

 ```
2. Install Required Libraries:
   ```
   pip install -r requirements.txt


## Quick Start

### Training
 ```
For P5 models:
  ```
  python tools/train.py --batch 32 --conf configs/yolov6s_finetune.py --data data/dataset.yaml --fuse_ab --device 0
  ```

For P6 models:
  ```
  python tools/train.py --batch 32 --conf configs/yolov6s6_finetune.py --data data/dataset.yaml --img 1280 --device 0


### Evaluation
   ```
   Reproduce mAP on COCO val2017 dataset:
   ```
  python tools/eval.py --data data/coco.yaml --batch 32 --weights yolov6s.pt --task val --reproduce_640_eval
  

### Inference
 ```
  Run inference on new images:
  ```
  python tools/infer.py --weights path/to/weights --source path/to/image --device 0
  

## Acknowledgments

This project utilizes the YOLOv6 object detection framework, originally developed by the team at Meituan. Full credit for the creation and initial development of the YOLOv6 model goes to the original authors. For more information on the base model and additional functionalities, visit the [official YOLOv6 repository](https://github.com/meituan/YOLOv6).

## License

This project is licensed under the GPL-3.0 License - see the LICENSE file for details.

## Contact

- Muhammad Salman - [Email_Adress](mailto:sm607795@gmail.com)
- Project Link: [https://github.com/MSalmanA95/Object-Detection-for-Public-Safety-using-YoloV6.git](https://github.com/MSalmanA95/Object-Detection-for-Public-Safety-using-YoloV6.git)

---

This README is structured to provide a clear overview of your project, how to get it running, and the necessary commands for training, evaluation, and inference. It also properly credits the original developers of the YOLOv6 model, ensuring their contributions are acknowledged you can directly acess colab code by downloading the zip file.
