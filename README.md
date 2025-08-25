# Acted-Emotional-Speech-Dynamic



## 📋 Project Overview

This project focuses on **emotion recognition in acted emotional speech** using dynamic analysis techniques. The goal is to develop a machine learning model that can accurately classify emotions from speech audio, with applications in human-computer interaction, mental health assessment, and entertainment technology.

## 🎯 Objectives

- **Emotion Classification**: Identify and classify emotions from speech audio
- **Dynamic Analysis**: Implement real-time or near real-time emotion detection
- **Feature Extraction**: Extract relevant acoustic features from speech signals
- **Model Development**: Build and train machine learning models for emotion recognition
- **Performance Evaluation**: Assess model accuracy across different emotion categories

## 🚀 Features

- **Multi-Emotion Classification**: Support for multiple emotion categories (e.g., happy, sad, angry, neutral, etc.)
- **Real-time Processing**: Dynamic analysis capabilities for live audio streams
- **Feature Engineering**: Advanced acoustic feature extraction from speech signals
- **Model Training**: Comprehensive training pipeline with validation
- **Performance Metrics**: Detailed evaluation and visualization of results

## 🛠️ Technologies Used

- **Python**: Core programming language
- **Jupyter Notebook**: Development and experimentation environment
- **Machine Learning Libraries**: 
  - Scikit-learn
  - TensorFlow/PyTorch (if applicable)
  - NumPy, Pandas
- **Audio Processing**: 
  - Librosa
  - PyAudio
  - SciPy
- **Data Visualization**: 
  - Matplotlib
  - Seaborn
  - Plotly


## 📂 Dataset

* **Source**: Acted Emotional Speech Dynamic Database
* **Format**: `.wav` audio files organized by emotion labels (e.g., *anger, happiness, sadness, neutral*).
* **Preprocessing**:

  * Audio resampled at **22,050 Hz**
  * Extracted **MFCC features** (13 coefficients)
  * Fixed-length sequences (padded or trimmed to 40 frames)

## 🧠 Model Architecture

* Input: `(40, 13)` MFCC feature sequences
* **LSTM layers** for temporal feature learning
* **Dense layer with ReLU** for hidden representation
* **Softmax output layer** for multi-class emotion classification

## 📊 Training Details

* Loss: `categorical_crossentropy`
* Optimizer: `Adam`
* Metrics: `accuracy`
* Split: `80% training / 20% testing`
* Epochs: `30`
* Batch size: `16`

## 📈 Results & Visualization

* Accuracy and loss curves plotted per epoch.
* Audio and MFCC plots for better interpretability.

## 🚀 How to Run

1. Mount Google Drive (if running on Colab).
2. Install dependencies:

   ```bash
   pip install librosa resampy tensorflow scikit-learn matplotlib
   ```
3. Place the AESD dataset in the correct path:

   ```
   /content/drive/MyDrive/Acted Emotional Speech Dynamic Database/
   ```
4. Run the notebook cells step by step.

## 🔮 Applications

* Human-computer interaction
* Emotion-aware virtual assistants
* Healthcare (stress/mood monitoring)
* Call center emotion analytics
