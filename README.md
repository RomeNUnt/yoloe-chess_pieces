# Chess Piece Detection using YOLOE

This project trains a YOLOE model to detect and classify white and black chess pieces on a chessboard
from images. The goal is to build a lightweight and accurate object detection system
suitable for tasks such as board state recognition.

---

##  Features
- Object detection of 12 chess piece classes (6 chess pieces for 2 colors, black and white)
- Trained using YOLOE
- Custom dataset with real-board images
- Evaluation metrics and confusion matrix included

---

##  Dataset
The full dataset is not included in this repository due to size constraints. However, a small sample of the images and labels have been provided in 'data/sample/'.

Download the full dataset from:
https://universe.roboflow.com/yolo-ja0zo/chess-pieces-kaid5/dataset/3

Expected structure:

data/
├── images/
│ ├── train/
│ └── val/
└── labels/
├── train/
└── val/

## Configurations

Key training parameters are documented in 'config/'

Default settings:
- Optimizer: AdamW (YOLO default)
- Learning rate: 0.01
- Batch size: 4
- Image size: 512
- Seed: default YOLO seed

## Training

Model Training was done using a Jupyter Notebook

To run:

1. Install dependencies
pip install -r requirements.txt

2. Launch Jupyter
jupyter notebook

3. Open and run
notebooks/yoloe.ipynb

## Evaluation

Key metrics are stored in 'results/metrics.json'.
A confusion matrix is stroed in 'results/confusion_matrix.png'.
Sample predictions along with its original image are kept in 'results/'.

## Notes

Model weights are not included due to GitHub file size limits
Training Outputs are ignored via .gitignore

## Authors

Roman Suksumit
Robotics and Automation Engineering