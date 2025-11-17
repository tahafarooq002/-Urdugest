# Urdugest

Urdugest is an AI-powered Urdu Sign Language recognition system. It detects Urdu alphabets from hand gestures and forms complete words in real-time.

## Project Structure
- `data/` - Original and preprocessed datasets
- `src/` - Source code (training, prediction, preprocessing)
- `models/` - Saved models and checkpoints
- `notebooks/` - Experiments and demos
- `tests/` - Unit tests for scripts
- `scripts/` - Helper scripts

## Installation
```bash
git clone <repository-url>
cd Urdugest
pip install -r requirements.txt
```

## Usage

Training:
```bash
python src/train.py
```

## Prediction:
```bash
python src/predict.py --image path_to_image

```
Run main project:
```bash
python src/main.py
```
Contributing

Open issues, pull requests are welcome.

Ensure tests pass before pushing changes.




Detailed File Explanation
data/

Stores all your dataset files.

raw/ → untouched images or videos from PSL dataset.

processed/ → preprocessed for training (resized images, normalized, augmented).

README.md → include dataset description, source link, classes, and structure.

src/

main.py → main entry point; can run training, testing, or live demo.

model.py → define neural network architectures (CNN, LSTM, Transformers).

preprocess.py → functions for resizing, normalization, encoding labels, augmentations.

train.py → script to train the model with options for epochs, batch size, optimizer.

predict.py → load trained model and predict on new images or live webcam feed.

utils.py → helper functions like accuracy metrics, plotting results, saving/loading checkpoints.

models/

Store trained models and checkpoints.

Include README.md describing model format (e.g., .h5, .pt) and usage.

notebooks/

Interactive notebooks for testing, visualization, and experiments.

Examples: exploratory.ipynb for dataset analysis, demo.ipynb for a live demo.

tests/

Unit testing scripts for verifying correctness.

Example: test_main.py tests if main.py runs without errors.

Use pytest for automated testing.
