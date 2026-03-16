# MNIST Digit Classification Using CNN

This project is a handwritten digit classification system built using TensorFlow and Keras. It trains a Convolutional Neural Network (CNN) on the MNIST dataset and predicts digits from uploaded input images.

## Project Overview

The main objective of this project is to classify handwritten digits from `0` to `9` using deep learning. The model is trained on the MNIST dataset, which contains grayscale images of handwritten digits. After training, the model is saved and then used to predict the digit from a user-uploaded image.

This project was implemented in Google Colab using Python and TensorFlow.

## Dataset

This project uses the **MNIST dataset**, which is directly available through `tf.keras.datasets.mnist`.

### Dataset Details
- 10 classes (`0` to `9`)
- 28 × 28 grayscale images
- 60,000 training images
- 10,000 testing images

## Technologies Used

- Python
- Google Colab
- TensorFlow
- Keras
- NumPy
- Matplotlib
- PIL (Python Imaging Library)

## Model Architecture

The model is built using a Sequential CNN architecture with the following layers:

- `Conv2D` with 32 filters and ReLU activation
- `MaxPooling2D`
- `Flatten`
- `Dense` layer with 128 neurons and ReLU activation
- `Dropout` layer
- `Dense` output layer with softmax activation

The model is compiled using:
- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy
- **Metric:** Accuracy

## Project Workflow

The project follows these main steps:

1. Load the MNIST dataset using TensorFlow
2. Reshape the image data to include the channel dimension
3. Normalize pixel values by dividing by 255
4. Convert class labels to categorical format
5. Build and compile the CNN model
6. Train the model for 10 epochs
7. Evaluate the model on test data
8. Save the trained model as `mnist_model.h5`
9. Upload a custom image for prediction
10. Resize and preprocess the uploaded image
11. Predict the digit using the saved model

## Input Image Prediction

After training, the project allows a user to upload a handwritten digit image. The image is:

- converted to grayscale
- resized to 28 × 28
- inverted for proper MNIST-style formatting
- normalized and reshaped
- passed to the trained model for prediction

The predicted digit is then displayed as output.

## Files in This Repository

- `mnist.ipynb` — Google Colab notebook
- `mnist.py` — Python script version
- `mnist_model.h5` — saved trained model
- output image(s) — sample prediction output
- `README.md` — project documentation

Update the filenames above if your repository uses different names.

## How to Run

1. Open the notebook in Google Colab or run the Python script locally
2. Install the required libraries
3. Train the model on the MNIST dataset
4. Save the trained model
5. Upload a digit image for testing
6. View the predicted digit output

## Output

The model is able to classify handwritten digits and can also predict digits from user-uploaded images after preprocessing.

## Conclusion

This project demonstrates a simple and practical implementation of CNN-based image classification using the MNIST dataset. It covers model training, evaluation, saving, and custom image prediction in a single workflow.