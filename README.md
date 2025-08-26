f# Pneumonia Detection with a CNN

Welcome! This project uses a Convolutional Neural Network (CNN) to detect pneumonia from X-ray images.

## What’s in this project?
- A trained model: `cnn_pneumonia_augmented.keras`
- (Optional) Example images or results

## What does it do?
The model looks at X-ray images and predicts if a person has pneumonia.

## How did I train it?
- Used lots of X-ray images (some with pneumonia, some healthy)
- Used Keras and TensorFlow (Python libraries)
- Trained the model to spot patterns in the images

## Want to use the model?
You’ll need Python and Keras.  
Here’s some example code to load it:

```python
from keras.models import load_model
model = load_model('cnn_pneumonia_augmented.keras')
```

---

Thanks for visiting!  
