# CodeAlpha_-Speech-Emotion-Recognition
Speech Emotion Recognition – CodeAlpha Internship Task 2
Speech Emotion Recognition – CodeAlpha Internship Task 2
 **Project Overview**
 
This project was developed as part of the CodeAlpha Machine Learning Internship. The goal was to build a model that can recognize human emotions from speech audio files using deep learning and audio signal processing techniques.

 **Objective**
 
To classify speech recordings into emotional categories such as happy, sad, angry, fearful, calm, neutral, disgust, and surprised using extracted audio features and a neural network.

 **Dataset**
 
🔹 Source
I used the RAVDESS Emotional Speech Audio dataset, which contains 1,440 high-quality .wav files recorded by 24 professional actors. Each file represents one of eight emotions at varying intensities.

🔹 How I Accessed It
Instead of uploading the dataset manually to Google Drive, I downloaded it directly into Google Colab using the Kaggle API. This method was faster and more efficient for handling large files (~1.09 GB).

 **Tools & Technologies**
 
Google Colab – for development and GPU acceleration

Python – core programming language

Librosa – audio feature extraction

Keras – deep learning model

Scikit-learn – preprocessing and evaluation

Matplotlib – visualization

 **Workflow Summary**
 
1. Environment Setup
Installed required libraries (librosa, soundfile, kaggle)

Configured Kaggle API using kaggle.json

2. Dataset Download
Used Kaggle CLI to download and unzip the RAVDESS dataset directly into Colab

3. Feature Extraction
Extracted rich audio features:

MFCCs (Mel-Frequency Cepstral Coefficients)

Chroma

Spectral Contrast

Tonnetz

4. Data Preparation
Encoded emotion labels

Normalized features using StandardScaler

Split data into training and testing sets

5. Model Architecture
Built a fully connected neural network with:

Dense layers

Dropout for regularization

BatchNormalization for stability

Used categorical_crossentropy loss and adam optimizer

6. Training & Evaluation
Trained the model with early stopping

Achieved 94% accuracy on the test set

Evaluated using precision, recall, F1-score, and classification report

7. Model Saving
Saved the trained model in .keras format

Stored the final model in Colab and optionally moved to Google Drive

 **Results**
 
Metric	Value
Accuracy	94%
Macro F1-Score	0.94
Weighted F1	0.94
The model performed consistently across all emotion classes, with high precision and recall for each category.

 **Repository Contents**
 
Speech_Emotion_Recognition.ipynb – full Colab notebook with code and outputs

README.md – this documentation

emotion_model_ravdess_enhanced.keras – saved model (optional)

