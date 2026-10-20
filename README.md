# Benchmarking YOLO-based deep learning models for Automated Detection of Root Nodules in Hybrid Bean (Phaseolus vulgaris L.) var. ICA Quimbaya

This project implements convolutional neural network (CNN)-based object detection models from the YOLO family for the automated detection and 
counting of root nodules in the ICA Quimbaya hybrid common bean variety. The study evaluates and compares three YOLO architectures: YOLOv8n, 
YOLO11, and YOLO26, considering their detection accuracy, computational efficiency, and inference performance. The objective is to assess 
their suitability for automated root nodule phenotyping and real-time object detection applications in agricultural systems.
 
<img width="996" height="650" alt="image" src="https://github.com/user-attachments/assets/8d9e0adf-a869-4091-8803-68fe163ce0bc" />

<img width="828" height="539" alt="image" src="https://github.com/user-attachments/assets/21e7e460-b430-4126-a323-d4ffadc04128" />

<img width="938" height="573" alt="image" src="https://github.com/user-attachments/assets/77ed99e2-29f5-45d1-8eb5-274fe25c3cdd" />

### Figure 1. (A) YOLOv8 architecture, (B) YOLOv11 architecture, and YOLO26 network architecture.

### Table 1. Taxonomy of architectural innovations in YOLOv8, YOLOv11, YOLO26.
<img width="1132" height="591" alt="image" src="https://github.com/user-attachments/assets/998a2dd4-3b12-45cf-ad39-7fa4b693cffa" />

## Model Training (YOLOv8n, YOLO11, YOLO26)
The original root nodule image dataset was constructed and comprised a total of 1,000 images. The dataset was divided into training (800 images),
validation (100 images), and test (100 images) using an 8:1:1 ratio. Manual annotation of the root nodules was performed using the commercial
Roboflow platform (Dataset of bean, 2026). Root nodules were delineated using circular regions of interest, while the root system itself was
excluded from the annotations. All images were acquired at an original resolution of 4032 × 3024 pixels and were subsequently resized according
to the input requirements of each YOLO architecture and stored in JPG format.
Following dataset preparation, the object detection models were developed using the annotated image dataset. The Google Colab environment was
configured to implement and train three YOLO-based architectures: YOLOv8n, YOLO11, and YOLO26. All models were trained under identical experimental
conditions to ensure a fair comparison among architectures. To promote methodological consistency, transparency, and reproducibility, the main 
training hyperparameters were kept constant across all experiments, including a learning rate of 0.01, a batch size of 16, and an initial training 
schedule of 50 epochs. During the training process, weight files were generated corresponding to the optimized parameters of each model. 
Table 2 presents a comparative summary of the YOLOv8n, YOLO11, and YOLO26 variants, including input size, number of layers, number of parameters,
and GFLOPs, thereby providing an overview of their architectural complexity.

### Table 2. Computational complexity of the YOLOv8n, YOLO11, and YOLO26 models
<img width="1096" height="228" alt="image" src="https://github.com/user-attachments/assets/3f184281-0396-42b6-b143-094db967a931" />

The comparative performance of the evaluated architectures is presented below. The analysis includes metrics related to detection accuracy,
computational efficiency, and real-time inference capability, allowing a comprehensive assessment of the performance of YOLOv8n, YOLO11, and
YOLO26 for root nodule identification in the ICA Quimbaya hybrid variety.

### Table 3. Comparative Performance of the Evaluated YOLO Architectures: YOLOv8n, YOLO11, and YOLO26.

<img width="1109" height="254" alt="image" src="https://github.com/user-attachments/assets/1550a394-3c07-4f61-896f-a584555e9daf" />













