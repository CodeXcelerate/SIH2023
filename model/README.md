# CNN Model for Predicting Medicinal Leaves and Raw Materials

This Convolutional Neural Network (CNN) model predicts the type of medicinal leaves and raw materials based on input images. The model is trained on a dataset of labeled images of various medicinal leaves and raw materials.

## Requirements

To run this model, you will need the following:

- Python 3.12
- TensorFlow 2.x
- NumPy
- Matplotlib
- Scikit-Learn
- LabelEncoder


## Usage

To use this model, follow these steps:

1. Clone this repository to your local machine.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the `predict.py` script with an input image to get a prediction.

## Model Architecture

The CNN model consists of several convolutional and pooling layers, followed by fully connected layers. Input images are first passed through convolutional layers, which extract features. The output of these layers is then passed through fully connected layers for classification into different categories.

## Dataset

The dataset used to train this model contains labeled images of various medicinal leaves and raw materials. The dataset was collected from diverse sources and preprocessed before being utilized for training.

## Results

The model achieved an accuracy of 95% on the test set, demonstrating its ability to accurately predict the type of medicinal leaves and raw materials based on input images.

## Credits

This model was developed by Shubham Tiwari as part of SIH1343. The dataset used to train the model was collected from various sources and preprocessed by devjster.