# Moving Vehicle Registration Number Detection

## Overview
This project is designed to detect and recognize vehicle registration numbers (license plates) from video footage. It employs object detection, tracking, and optical character recognition (OCR) to identify vehicles, track them, and extract text from license plates.

## Project Structure
Here's an overview of the key files and their roles in the repository:

- **main.py**: Main script for processing video, detecting vehicles, and extracting license plate text.
- **sort.py**: Implementation of the SORT (Simple Online and Realtime Tracking) algorithm.
- **best.pt**: Pre-trained YOLOv8 model for license plate detection.
- **kia_alto.mp4**: Sample video for testing the detection workflow.
- **README.md**: Project documentation (this file).

## Methodology

### Training Data Set
The detection model was trained using the License Plate Recognition Dataset from Roboflow Universe, containing over 24,000 annotated images of license plates. This dataset offers a diverse range of conditions, providing robust training for real-world applications. The model uses YOLOv8 for its high accuracy and speed in real-time applications.

### Vehicle Detection with YOLOv8
YOLOv8n is applied to each frame in the video to detect vehicles. The model divides each frame into a grid, predicting bounding boxes and class probabilities for various vehicle types, including cars, trucks, buses, motorcycles, and bicycles. The output includes bounding boxes and class probabilities, with visual representation on the video frame.


