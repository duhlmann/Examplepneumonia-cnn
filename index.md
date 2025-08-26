# Pneumonia Detection with a CNN

Welcome! This project uses a Convolutional Neural Network (CNN) to detect pneumonia from X-ray images.

## What's in this project?

- **Trained Model:** `cnn_pneumonia_augmented.keras`
- *(Optional)* Example images or results (add if available)

## What does it do?

The model analyzes X-ray images and predicts if a person has pneumonia.

## How did I train it?

- Used a large dataset of X-ray images (both with and without pneumonia)
- Utilized Keras and TensorFlow (Python libraries)
- Trained the model to spot patterns indicating pneumonia

## Getting Started

### Requirements

- Python 3.x
- TensorFlow
- Keras
- (Optional) NumPy, Matplotlib (for image handling and visualization)

### Loading the Model

```python
from tensorflow import keras

model = keras.models.load_model('cnn_pneumonia_augmented.keras')
```

### Making Predictions

```python
import numpy as np
from tensorflow import keras
from PIL import Image

# Load and preprocess image (resize to model input size, e.g., 224x224)
img = Image.open('your_xray_image.jpg').resize((224, 224)).convert('L')
img_array = np.array(img) / 255.0
img_array = img_array.reshape(1, 224, 224, 1)  # Adjust shape as needed

prediction = model.predict(img_array)
print("Pneumonia probability:", prediction[0][0])
```

## Want to use the model?

Clone this repo, install the requirements, and follow the code above to make predictions on your own images!

---

Feel free to add information about your dataset, training process, results, or how to contribute.
