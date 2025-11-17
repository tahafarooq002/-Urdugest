Urdugest

Urdugest is an AI-powered Urdu Sign Language recognition system. It detects Urdu alphabets from hand gestures and forms complete words in real-time, helping bridge communication for Urdu sign language users.

Project Structure
Urdugest/
│
├── data/                   # Original and preprocessed datasets
│   ├── raw/                # Raw/untouched images or videos from the PSL dataset
│   ├── processed/          # Preprocessed data (resized, normalized, augmented)
│   └── README.md           # Dataset details: source, format, classes
│
├── src/                    # Source code
│   ├── __init__.py
│   ├── main.py             # Main script to run training, prediction, or live demo
│   ├── model.py            # Neural network architectures (CNN, LSTM, Transformer)
│   ├── preprocess.py       # Data preprocessing functions
│   ├── train.py            # Training script (with options for epochs, batch size, optimizer)
│   ├── predict.py          # Load trained models and predict on images or live webcam feed
│   └── utils.py            # Helper functions: metrics, plotting, saving/loading checkpoints
│
├── models/                 # Trained models and checkpoints
│   ├── checkpoints/        # Intermediate saved models during training
│   └── README.md           # Description of model files and formats (.h5, .pt)
│
├── notebooks/              # Jupyter notebooks for experiments and demos
│   ├── exploratory.ipynb   # Dataset analysis and visualization
│   └── demo.ipynb          # Demo of real-time recognition
│
├── tests/                  # Unit tests for scripts
│   ├── test_main.py        # Test main script runs correctly
│   ├── test_model.py       # Test model architecture and forward pass
│   └── test_utils.py       # Test helper functions
│
├── scripts/                # Optional helper scripts
│   └── download_data.py    # Script to download or prepare datasets
│
├── requirements.txt        # Python dependencies
├── README.md               # Project description (this file)
├── .gitignore              # Files/folders to ignore in Git
├── LICENSE                 # License (e.g., MIT)
└── setup.py                # Optional setup for packaging

Installation

Clone the repository and install dependencies:
```bash
git clone <repository-url>
cd Urdugest
pip install -r requirements.txt
```
Usage
Training
```bash
python src/train.py
```
Prediction
python src/predict.py --image path_to_image

Run Main Project
```bash
python src/main.py
```
Contributing

Open issues or submit pull requests.

Ensure all tests pass before pushing changes.

Detailed File Explanation

data/ – Stores all dataset files:

raw/ → Original PSL Urdu alphabet images or videos.

processed/ → Preprocessed dataset for training (resized, normalized, augmented).

README.md → Includes dataset details: source, format, classes.

src/ – Source code for training, prediction, and preprocessing:

main.py → Entry point for running training, testing, or demo.

model.py → Define neural network architectures (CNN, LSTM, Transformers).

preprocess.py → Data preprocessing: resizing, normalization, label encoding, augmentation.

train.py → Script to train models with configurable epochs, batch size, optimizer.

predict.py → Load trained models and make predictions on new images or webcam input.

utils.py → Helper functions: metrics, plotting, saving/loading checkpoints.

models/ – Store trained models and checkpoints.

Include README.md explaining file formats (.h5, .pt) and usage.

notebooks/ – Interactive experiments and demos:

exploratory.ipynb → Dataset analysis and visualization.

demo.ipynb → Demo of real-time Urdu gesture recognition.

tests/ – Unit tests to verify correctness:

test_main.py → Test main script runs without errors.

test_model.py → Test model structure and forward pass.

test_utils.py → Test helper functions.

scripts/ – Optional helper scripts, e.g., dataset downloading.

requirements.txt – All Python dependencies.
