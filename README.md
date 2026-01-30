# Single-Digit-Classifier-ML-Model
A real-time handwritten digit recognition application using a CNN model trained on the MNIST dataset. Draw digits on a canvas and get instant predictions.

## Features
- Real-time digit prediction as you draw
- Interactive drawing canvas using Pygame
- CNN model trained on MNIST dataset
- Single digit recognition (0-9)

## Tech Stack
- **Python 3.11**
- **TensorFlow/Keras** - Model training and inference
- **Pygame** - GUI and drawing interface
- **OpenCV** - Image preprocessing
- **NumPy** - Array operations

## How It Works
1. Draw a digit on the canvas using your mouse
2. Release the mouse button to trigger prediction
3. The model preprocesses the drawn digit to match MNIST format (28x28 grayscale)
4. CNN model predicts the digit and displays the result on screen
5. Press 'n' to clear the canvas and draw again

## Project Structure
```
.
├── app.py              # Main application with GUI and prediction logic
├── OCR.ipynb           # Model training notebook
├── bestmodel.h5        # Trained CNN model
└── README.md
```

## Installation
Clone the repository:
```bash
git clone https://github.com/yourusername/single-digit-classifier-ML-model.git
cd single-digit-classifier-ML-model
```

Install dependencies:
```bash
pip install pygame numpy opencv-python keras tensorflow
```

## Running the Application
Make sure `bestmodel.h5` is in the project directory, then run:
```bash
python app.py
```

## Controls
- **Mouse drag** - Draw on the canvas
- **Mouse release** - Trigger prediction
- **N key** - Clear the canvas

## Limitations
- Recognizes single digits only (0-9)
- Model accuracy depends on drawing quality and centering
- Works best with digits similar to MNIST handwriting style

## Model Training
The CNN model was trained using the MNIST dataset. Training code is available in `OCR.ipynb`. The model achieves standard MNIST accuracy for single digit classification.
