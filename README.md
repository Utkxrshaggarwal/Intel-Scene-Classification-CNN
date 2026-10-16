# Intel Scene Classification using CNN

A Convolutional Neural Network built with TensorFlow/Keras that classifies
natural scene images into six categories: **buildings, forest, glacier,
mountain, sea, and street**.

## Dataset
[Intel Image Classification](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)
from Kaggle, with about 25,000 images (150x150 pixels) split into training and test sets.

## Model
- 4 convolution blocks (Conv2D → BatchNormalization → MaxPooling)
- Global average pooling, a dense layer, dropout (0.5) and a softmax output
- Data augmentation (flip, rotation, zoom) to reduce overfitting
- Adam optimizer with early stopping and learning-rate reduction

## Results
- Test accuracy: **XX%**
- Evaluated with a classification report and confusion matrix

## How to run
Click the badge below to open the notebook in Google Colab, enable a GPU
(Runtime > Change runtime type > T4 GPU) and run all cells.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/Intel-Scene-Classification-CNN/blob/main/intel_image_cnn_colab.ipynb)

## Tech stack
Python, TensorFlow/Keras, NumPy, Matplotlib, Seaborn, scikit-learn

## Future improvements
- Transfer learning with MobileNetV2 / ResNet50
- Hyperparameter tuning
- Deploy as a web app (Streamlit or Gradio)
