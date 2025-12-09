# Simple-Image-Classifier

A simple Convolutional Neural Network (CNN) for MNIST handwritten digit classification using TensorFlow / Keras.

## What’s included
- `Simple-Image-Classifier.ipynb` — notebook with data loading, preprocessing, CNN definition, training, evaluation, and model saving.
- `OpenCV-Demo.ipynb` — small demo that applies OpenCV preprocessing to a test image and runs inference using the saved model.
- `models/mnist_cnn.h5` and `models/mnist_cnn.keras` — saved trained models (best checkpoint and native Keras format).
- `requirements.txt` — Python packages used.

## How to run (local)
1. Create and activate venv:
   ```bash
   python -m venv venv
   # Windows
   .\venv\Scripts\activate

   # macOS/Linux
   source venv/bin/activate
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run `Simple-Image-Classifier.ipynb` cells top → down. The trained model will be saved to `models/`.

4. Run `OpenCV-Demo.ipynb` to test the saved model.

   This notebook:
   - Loads the trained model from `models/`
   - Applies OpenCV preprocessing (resize → blur → resize)
   - Runs inference on a sample MNIST test image
   - Displays original, processed, and predicted outputs
