# Speech Emotion Recognition System 🎙️

This project is a **Speech Emotion Recognition System** that uses a **Convolutional Neural Network (CNN)** to classify human emotions such as **happy, sad, neutral, angry**, and more based on voice inputs. The system also provides real-time audio recording functionality for testing emotions instantly.

---

## Features 🚀

- **Emotion Detection**: Accurately detects emotions from pre-recorded or real-time audio.
- **Real-time Audio Recording**: Allows users to record their voice and predict the emotion live.
- **Dataset Support**: Trained on **RAVDESS** and **SAVEE** datasets for diverse emotional expressions.
- **Custom Testing**: Users can evaluate their own audio files.
- **Model Training**: Trains a CNN model from scratch using the provided datasets.

---

## Datasets Used 📊

### 1. **RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**

- Contains **24 professional actors** (12 male, 12 female) speaking in a North American accent.
- Includes **eight emotional states**: calm, happy, sad, angry, fearful, disgust, surprised, and neutral.
- Files are in `.wav` format and labeled systematically for easy identification.

More about RAVDESS: [Link to RAVDESS Dataset](https://zenodo.org/record/1188976)

### 2. **SAVEE (Surrey Audio-Visual Expressed Emotion)**

- Consists of recordings from **four male actors** expressing **seven emotions**: anger, disgust, fear, happiness, sadness, surprise, and neutral.
- Files are also in `.wav` format and labeled accordingly.

More about SAVEE: [Link to SAVEE Dataset](http://kahlan.eps.surrey.ac.uk/savee/)

---

## How to Run 🖥️

### Prerequisites

Make sure you have the following installed:

1. **Python** (>= 3.7)
2. Libraries:
   - **TensorFlow**: `pip install tensorflow`
   - **NumPy**: `pip install numpy`
   - **Librosa**: `pip install librosa`
   - **Matplotlib**: `pip install matplotlib`
   - **Sklearn**: `pip install scikit-learn`
   - **SoundDevice**: `pip install sounddevice`

   Install them all together:
   ```bash
   pip install tensorflow numpy librosa matplotlib scikit-learn sounddevice
## Steps to Run 🖥️

### 1. Train the Model:

- Use the `final_result_gender_test.ipynb` file to train the model.
- The script will:
  - Load and preprocess audio files from the **RAVDESS** and **SAVEE** datasets.
  - Train a CNN model on the processed data.
  - Save the trained model and its architecture as `.h5` and `.json` files respectively.

#### Run the following command:
```bash
python final_result_gender_test.ipynb***
```


### 2. Real-Time Audio Testing:
-Use the `Audio_recorder.ipynb` file to record real-time audio.
-The script will:
 -Record your voice using your system's microphone.
 -Save the recorded audio as a .wav file.
 -Predict the emotion using the trained model.
###Run the following command:
```bash

python Audio_recorder.ipynb
```
