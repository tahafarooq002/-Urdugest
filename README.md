## Urdugest

Urdugest is an AI-powered Urdu Sign Language recognition system. It detects Urdu alphabets from hand gestures and forms complete words in real-time, helping bridge communication for Urdu sign language users.

## Project StructureUrdugest – Urdu Sign Language Recognition

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/Urdugest-green)
![Status](https://img.shields.io/badge/Project-Active-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Jupyter%20Notebook-orange)



Urdugest is an AI-powered system that recognizes Urdu Sign Language (PSL) gestures and converts them into Urdu text in real-time. It detects alphabets, predicts words, and helps bridge communication gaps.

## 🚀 Features

#✋ Urdu Sign Detection – Detect hand gestures for Urdu alphabets

🧹 Preprocessing Pipeline – Resize, normalize, augment images

🤖 AI Prediction – Recognize alphabets using CNN/LSTM/Transformer

📝 Word Formation – Combine predicted alphabets into words

📊 Visualization & Logging – See predictions and model outputs

📓 Fully implemented in: src/main.py, notebooks/demo.ipynb

## 🛠️ Technologies Used
Tool	Purpose
Python	Main programming language
PyTorch	Model training & inference
OpenCV	Image processing & preprocessing
NumPy / Pandas	Computation & data handling
Matplotlib / Seaborn	Visualization
Jupyter Notebook	Experiments and demo
## 📁 Project Structure
Urdugest/
│
├── data/                   # Original & preprocessed datasets
│   ├── raw/                # Raw PSL dataset
│   ├── processed/          # Resized, normalized, augmented
│   └── README.md           # Dataset details
│
├── src/                    # Source code
│   ├── main.py             # Entry point
│   ├── train.py            # Training script
│   ├── predict.py          # Prediction script
│   ├── model.py            # Model definitions
│   ├── preprocess.py       # Preprocessing functions
│   └── utils.py            # Helper functions
│
├── models/                 # Trained models & checkpoints
│   └── README.md
│
├── notebooks/              # Jupyter notebooks
│   ├── exploratory.ipynb
│   └── demo.ipynb
│
├── tests/                  # Unit tests
│   ├── test_main.py
│   ├── test_model.py
│   └── test_utils.py
│
├── scripts/                # Helper scripts (e.g., dataset download)
├── assets/                 # Logo, sample input/output
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore

## ▶️ How to Run
## 1️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
## 2️⃣ Run Training

```bash
python src/train.py
```
## 3️⃣ Predict on New Image or Video
```bash
python src/predict.py --image path_to_image
```
## 4️⃣ Run Main Program
```bash
python src/main.py
```
##💡 Example Pipeline

Load image/video of hand gestures

Detect hand signs

Preprocess the image (resize, normalize, augment)

Predict alphabet using trained AI model

Form complete word from predicted alphabets

Display results

## 🛠️ Future Improvements

Deep learning gesture detection (YOLO, MediaPipe)

Real-time webcam support with low latency

Custom dataset expansion & augmentation

Multi-language support for regional sign languages

Unit tests & CI/CD workflow

requirements.txt – All Python dependencies.
