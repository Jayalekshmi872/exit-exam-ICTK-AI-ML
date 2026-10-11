# Bharatanatyam Mudra Recognition Using CNN

## 1. Project Overview

This project develops an image-classification system to recognize five Bharatanatyam hand mudras using a Convolutional Neural Network (CNN).

The application allows users to upload a hand image and receive a predicted mudra class, a confidence score, and the model's probability distribution across all five classes.

## 2. Mudra Classes

The model classifies images into five classes:

* Musti
* Pataka
* Sikhara
* Simhamukha
* Trisula

## 3. Dataset

The dataset contains 2,000 images, with 400 images per class.

The images were organized into training, validation, and test sets using a 70:15:15 split:

* Training: 1,400 images
* Validation: 300 images
* Testing: 300 images

The dataset was resized to 128 × 128 pixels for CNN training.

## 4. Model Architecture

A custom CNN was developed using:

* Rescaling
* Convolutional layers
* Max-pooling layers
* Flatten
* Dense layer
* Dropout
* Softmax output layer

The model was trained using the Adam optimizer and sparse categorical cross-entropy loss.

Actual test metrics should be reported here after final model evaluation.

## 5. Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn
* Streamlit
* Pillow

## 6. Project Structure

```text
Bharatanatyam-Mudra-Recognition/
├── mudra_recognition.ipynb
├── app.py
├── mudra_cnn.keras
├── requirements.txt
├── README.md
└── screenshots/
```

## 7. Installation

Install Python and open a terminal in the project directory.

Install the required packages:

```bash
pip install -r requirements.txt
```

## 8. Run the Application

Start the Streamlit application:

```bash
streamlit run app.py
```

Open the local address displayed in the terminal.

Upload a JPG, JPEG, or PNG image to receive a prediction.

## 9. Model Evaluation

The notebook evaluates the model using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion matrix
* Misclassified image analysis

The final test metrics and findings should be added here after evaluation.

## 10. Screenshots

The `screenshots/` directory contains dataset previews, exploratory visualizations, model training curves, classification results, and Streamlit application screenshots.

## 11. Limitations

The model predicts only the five classes represented in its training dataset. It may misclassify images with unusual backgrounds, poor lighting, unclear hand positions, or gestures outside the supported classes.

Prediction confidence is not a guarantee of correctness.

## 12. Future Improvements

* Add more diverse and accurately labelled training images.
* Evaluate transfer-learning architectures such as MobileNetV2.
* Improve performance on visually similar mudras.
* Add visual reference images to support student learning.
