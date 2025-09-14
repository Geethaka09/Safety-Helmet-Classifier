# Safety Helmet Detection using CNN

This project contains a Jupyter Notebook for building and training a Convolutional Neural Network (CNN) to detect whether a person in an image is wearing a safety helmet. The model is built using TensorFlow and Keras.

## Project Overview

The notebook covers the entire workflow of a deep learning project:
1.  **Data Loading and Preprocessing**: Loads an image dataset from Google Drive and uses `ImageDataGenerator` for data augmentation and splitting into training and validation sets.
2.  **Model Building**: Defines a sequential CNN model with multiple convolutional, max-pooling, and dense layers.
3.  **Model Training**: Compiles and trains the model on the dataset.
4.  **Model Evaluation**: Evaluates the model's performance using metrics like accuracy, loss, precision, recall, F1-score, and ROC/AUC. It also visualizes the training history and confusion matrix.
5.  **Prediction**: Includes a section to test the trained model on a single image and display the prediction.

## How to Use

1.  **Prerequisites**: Ensure you have a Google account with access to Google Colab and Google Drive.
2.  **Dataset**:
    *   Upload your image dataset to a folder in your Google Drive. The dataset should be structured with subdirectories for each class (e.g., `Yes` for images with helmets, `No` for images without).
    *   Update the `dataset_path` variable in the notebook to point to your dataset's location in Google Drive.
3.  **Dependencies**:
    *   Open the `helmet_classifier.ipynb` notebook in Google Colab.
    *   You can install the required libraries by running the following command in a Colab cell, or if running locally, by using the `requirements.txt` file.
        ```bash
        pip install -r requirements.txt
        ```
4.  **Running the Notebook**:
    *   Execute the cells in the notebook sequentially.
    *   You will be prompted to mount your Google Drive to give Colab access to your dataset.
    *   The notebook will train the model, save the trained model file (`.keras`) to your Google Drive, and display the evaluation results.

## File Structure
- `helmet_classifier.ipynb`: The main Jupyter Notebook with all the code.
- `requirements.txt`: A list of Python packages required for this project.
- `README.md`: This file.