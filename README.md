# Hand Gesture Recognition System

A real-time hand gesture recognition system using OpenCV, cvzone, and TensorFlow with a CNN model (DepthwiseConv2D).
Captures hand gestures through webcam and classifies them into predefined categories (e.g., A, B, C).

## Features
🖐️ Real-time hand detection using cvzone

✂️ Automatic cropping, resizing, and white background adjustment

🔍 CNN-based gesture classification (DepthwiseConv2D)

📸 Built-in data collection for training your own gestures

🧠 Customizable gesture labels (A, B, C, etc.)

## Tech Stack
Component	Library / Tool
Hand Detection	cvzone.HandTrackingModule
Model Framework	TensorFlow, Keras
CNN Layer	DepthwiseConv2D
Image Processing	OpenCV, NumPy
Classifier	cvzone.ClassificationModule
IDE (Optional)	VS Code, Jupyter

## Folder Structure
```
Hand-Gesture-Recognition/
│
├── Data/                  # Collected gesture images
├── Model/                 # keras_model.h5 and labels.txt
├── dataCollection.py      # Data collection script
├── test.py                # Gesture detection and classification
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
```
🔧 Setup Instructions (Local)
1. Clone the repository
```
git clone https://github.com/kjayasravani/Hand-Gesture-Recognition.git
cd Hand-Gesture-Recognition
```
2. Create a virtual environment
```
python -m venv venv
# Activate virtual environment
# Windows:
venv\Scripts\activate
```
3. Install dependencies
```
pip install -r requirements.txt
```

Press s to save a cropped, resized image into the Data/ folder.

🖥️ Run the Gesture Recognition App
Run the recognition script:

```
python test.py
```
Shows real-time detection and gesture prediction.

Recognizes gestures like A, B, C using your trained model.

## Model Details
CNN architecture with DepthwiseConv2D for lightweight and efficient processing.

Model file: Model/keras_model.h5

Labels file: Model/labels.txt

## Example Labels
```
labels = ["A", "B", "C"]
```
Add your own classes as needed and retrain the model.

## Recommended Best Practices
✅ Keep large datasets and trained models in separate storage if the repo grows big.

✅ Use a .gitignore file to exclude unnecessary folders like .venv/, __pycache__/, etc.

✅ Store model training scripts separately if you build your own models.
