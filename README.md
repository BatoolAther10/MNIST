
# MNIST Handwritten Digit Classification

This project is a handwritten digit classification system built using Python and deep learning. It uses the MNIST dataset and was implemented in Google Colab.

## About the Project

The aim of this project is to classify handwritten digits from 0 to 9. The model is trained on image data and learns to identify the correct digit based on patterns in the input images.

MNIST is a standard dataset in machine learning and is commonly used for learning image classification concepts. In this project, the dataset was loaded directly using TensorFlow/Keras, so no separate dataset download was required.

## Tools and Technologies

- Python
- Google Colab
- TensorFlow / Keras
- NumPy
- Matplotlib

## Files in this Repository

- `MNIST.ipynb` – notebook version of the project
- `mnist.py` – python script version
- `output.jpg` or output file – sample output
- `report.pdf` – project report
- `README.md` – project documentation

## Dataset

This project uses the MNIST handwritten digit dataset, which contains grayscale images of digits from 0 to 9.

- 10 classes
- 28 × 28 pixel images
- 60,000 training images
- 10,000 test images

The dataset is available directly through TensorFlow/Keras.

## Project Workflow

The main steps followed in this project are:

1. Load the MNIST dataset
2. Preprocess and normalize the image data
3. Build the model
4. Train the model
5. Evaluate the model performance
6. Display and save the results

## Result

The model was trained and tested for handwritten digit classification, and the output shows that it can successfully predict digit classes from image input.

## Conclusion

This project helped in understanding the basic workflow of deep learning for image classification, including preprocessing, model training, and evaluation using the MNIST dataset.