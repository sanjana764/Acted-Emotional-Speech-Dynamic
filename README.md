# Acted-Emotional-Speech-Dynamic



## 📌 Project Overview

This project builds a **Speech Emotion Recognition (SER) model** using the **Acted Emotional Speech Dynamic Database**. The system extracts **MFCC features** from audio files and trains a **deep learning model (LSTM-based)** to classify emotions such as anger, happiness, sadness, and others from speech.

## 📂 Dataset

* **Source**: Acted Emotional Speech Dynamic Database
* **Format**: `.wav` audio files organized by emotion labels (e.g., *anger, happiness, sadness, neutral*).
* **Preprocessing**:

  * Audio resampled at **22,050 Hz**
  * Extracted **MFCC features** (13 coefficients)
  * Fixed-length sequences (padded or trimmed to 40 frames)

## ⚙️ Features Extracted

* **MFCCs (Mel-Frequency Cepstral Coefficients)**
* Waveform and MFCC visualizations included for analysis.

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
