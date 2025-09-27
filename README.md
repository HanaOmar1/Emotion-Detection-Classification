# 🎤 Real-Time Speech Emotion Detection with Gemini LLM Fallback

## Overview
This project is a **real-time speech emotion recognition system** that combines classical machine learning with the **Google Gemini LLM** to classify emotions in spoken text. Users can speak directly into their microphone and instantly see the recognized text and predicted emotion.

- **Speech-to-Text Conversion:** Uses Python’s `speech_recognition` to transcribe microphone input.
- **Machine Learning Prediction:** Uses a **Logistic Regression model** trained with **NLP preprocessing** and **TF-IDF vectorization**. The model achieved **~90% accuracy** on the test set and predicts five emotions: happy, sad, angry, neutral, surprised.
- **LLM Fallback:** Automatically uses **Google Gemini LLM (gemini-2.5-pro)** if the ML model confidence is below a threshold.
- **Interactive UI:** Built with **Gradio**, providing a clean and user-friendly interface.
- **Confidence-Aware:** Displays prediction confidence and indicates when Gemini fallback is used.

---

## Features
- Real-time microphone input
- Emotion classification with confidence check
- Logistic Regression model with NLP preprocessing and TF-IDF
- Automatic fallback to Gemini LLM
- Interactive, browser-based interface

---

## Demo
<img width="1889" height="884" alt="image" src="https://github.com/user-attachments/assets/8f0b63c8-264e-4b8e-9d1e-79486c4d4725" />

---

## Technologies Used
- Python 3.11
- scikit-learn (Logistic Regression, TF-IDF)
- NLP preprocessing techniques (cleaning, tokenization)
- Gradio
- SpeechRecognition
- joblib
- Google Gemini LLM (`google-genai`)
