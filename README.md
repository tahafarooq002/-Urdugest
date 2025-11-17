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
