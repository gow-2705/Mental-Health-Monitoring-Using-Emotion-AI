# 🧠 Mental Health Monitoring Using Emotion AI

## 📌 Project Overview

This project is an AI-based system that analyzes emotional states using facial expressions, voice, and text inputs. It uses deep learning for facial emotion classification and sentiment analysis for text and voice inputs. The system provides an interactive web-based dashboard for displaying the detected emotions.

## 🚀 Features

* Real-time facial emotion detection using a webcam
* Facial emotion classification using a trained CNN (Convolutional Neural Network) model
* Facial emotion detection from uploaded images
* Voice input analysis using speech recognition and sentiment analysis
* Text-based emotion detection using sentiment analysis
* Supports facial emotions such as Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral
* Displays Face, Voice, Text, and Overall emotion results
* Interactive web-based dashboard using Streamlit

## 🛠️ Technologies Used

* Python
* Natural Language Processing (NLP)
* OpenCV
* TensorFlow / Keras
* NumPy
* Streamlit
* Streamlit-WebRTC
* TextBlob
* SpeechRecognition
* PyDub

## 🧠 Model Details

The facial emotion detection module uses a trained Convolutional Neural Network (CNN) model stored in `emotion_model.h5`.

OpenCV Haar Cascade is used to detect faces from uploaded images and live webcam frames. The detected face is converted to grayscale, resized to 64 × 64 pixels, normalized, and passed to the CNN model for emotion classification.

The facial emotion categories include:

* Angry
* Disgust
* Fear
* Happy
* Sad
* Surprise
* Neutral

For text and voice inputs, TextBlob sentiment polarity is used to classify the emotional state as Happy, Sad, or Neutral.

## 📸 Output

The system provides:

* Facial emotion detection from uploaded images
* Real-time facial emotion detection through a webcam
* Voice-to-text conversion followed by sentiment-based emotion analysis
* Text-based emotion analysis
* An emotion dashboard displaying Face, Voice, Text, and Overall results

## ⚙️ How It Works

### 🙂 Face Emotion Detection

1. The user uploads an image or enables the live camera.
2. OpenCV Haar Cascade detects the face.
3. The detected face is converted to grayscale and resized to 64 × 64 pixels.
4. The trained CNN model predicts the facial emotion.
5. The predicted emotion is displayed on the dashboard.

### 🎤 Voice Emotion Analysis

1. The user uploads a voice file.
2. The audio is converted into WAV format.
3. SpeechRecognition converts the voice into text.
4. TextBlob analyzes the sentiment polarity of the converted text.
5. The system classifies the result as Happy, Sad, or Neutral.

### ✍️ Text Emotion Analysis

1. The user enters text into the application.
2. TextBlob calculates the sentiment polarity.
3. The system classifies the emotional state as Happy, Sad, or Neutral.
4. The result is displayed on the dashboard.

## 📂 Project Structure

* `app.py` → Main Streamlit application
* `emotion_model.h5` → Trained CNN model for facial emotion classification
* `haarcascade_frontalface_default.xml` → Haar Cascade classifier for face detection
* `Assets/` → Sample images and audio files
* `README.md` → Project documentation

## ▶️ How to Run

1. Install the required dependencies:

```bash
pip install streamlit opencv-python tensorflow numpy streamlit-webrtc av textblob pydub SpeechRecognition
```

2. Run the Streamlit application:

```bash
streamlit run app.py
```

3. Open the Streamlit interface in your browser.

4. Select the Face, Voice, or Text module and provide the required input.

## 🎯 Applications

* Emotion-aware AI systems
* Mental health awareness and monitoring support
* Human-computer interaction
* Emotion analysis applications
* Healthcare support systems

## 🔮 Future Improvements

* Improve facial emotion classification accuracy
* Add more emotion categories
* Improve voice emotion analysis using audio features
* Add historical emotion tracking and visualization
* Enhance the dashboard with detailed analytics
* Deploy the application as a web-based service

## 👩‍💻 Author

Gowthamee G
