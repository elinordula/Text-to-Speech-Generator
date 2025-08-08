# Text-to-Speech-Generator

Text-to-Speech Generator
Overview
This project is a simple yet powerful Text-to-Speech (TTS) tool that converts input text into human-like speech using a pre-trained deep learning model. It is built using the open-source Coqui TTS library and provides a clean, interactive interface powered by Gradio.

Users can type any sentence and instantly hear it spoken aloud in a natural-sounding voice — all in one click, with no coding required.

Model Used
The TTS model used in this project is:

tts_models/en/ljspeech/tacotron2-DDC from Coqui TTS

It is trained on the LJ Speech Dataset, featuring a female American English speaker

The model uses Tacotron2 for spectrogram generation and a vocoder for waveform synthesis

Features
The current version of this project supports:

🔊 Convert any English text into high-quality speech

🧑‍💻 Simple, browser-based user interface using Gradio

📁 Instant audio playback with no extra tools needed

💬 Real-time TTS generation using a pre-trained model

✅ Fully runnable in Google Colab or locally

How It Works
Model Loading
The Tacotron2-DDC model is loaded once using the Coqui TTS API.

Text Processing
The user enters text using the Gradio UI.

TTS Conversion
The model generates a .wav audio file from the input text.

Audio Output
The Gradio app plays back the generated audio instantly.

Gradio Interface
A simple web-based UI was created using Gradio.
Users can:

✍️ Type or paste any sentence

▶️ Click a button to generate audio

🎧 Listen to the AI-generated speech in the browser

Example Inputs
Text Input	Output Voice
Hello! I hope you're having a great day.	Human-like female voice (LJ Speech)
Wow, that was absolutely amazing!	Expressive English narration
Once upon a time, in a land far, far away...	Storytelling tone, natural-sounding

Tools and Libraries Used
Python

Coqui TTS – for speech generation

Gradio – for the web-based user interface

Google Colab – for browser-based testing and deployment

Planned Features (Coming Soon)
Feature	Description
📥 Audio Download	Allow users to download the generated .wav file
🎛️ Speed Control	Adjust the speaking rate of the TTS output
🌍 Multilingual Support	Add support for multiple languages and accents
🧑‍🎤 Voice Cloning	Clone your voice from a short audio sample
🎨 Custom UI Theme	Improve layout with dark mode and modern styling

How to Run
Install Dependencies

bash
Copy
Edit
pip install TTS gradio
Run the App

bash
Copy
Edit
python app.py
Or Launch in Colab

python
Copy
Edit
interface.launch()
