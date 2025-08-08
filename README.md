# Text-to-Speech Generator

## Overview

This project is a simple yet powerful **Text-to-Speech (TTS)** tool that converts input text into human-like speech using a pre-trained deep learning model. It is built using the open-source **Coqui TTS** library and provides a clean, interactive interface powered by **Gradio**.

Users can type any sentence and instantly hear it spoken aloud in a natural-sounding voice — all in one click, with no coding required.

---

## Model Used

The TTS model used in this project is:

- `tts_models/en/ljspeech/tacotron2-DDC` from Coqui TTS  
- Trained on the **LJ Speech Dataset**, which contains recordings of a female American English speaker  
- Uses **Tacotron2** for spectrogram generation and a **vocoder** for waveform synthesis

---

## Features

The current version supports:

- Convert English text into high-quality speech
- Simple, browser-based user interface using Gradio
- Instant audio playback with no extra tools needed
- Real-time speech generation using a pre-trained model
- Compatible with Google Colab and local environments

---

## How It Works

1. **Model Loading**  
   The Tacotron2-DDC model is loaded once using the Coqui TTS API.

2. **Text Processing**  
   The user enters text into the Gradio interface.

3. **TTS Conversion**  
   The model generates a `.wav` file from the input text.

4. **Audio Output**  
   The audio is played back in the browser using Gradio.

---

## Gradio Interface

A simple web-based interface is created using Gradio.  
Users can:

- Type or paste any sentence
- Click a button to generate audio
- Listen to the AI-generated voice instantly
- Can Increase the speed and also can download the audio clip.

---

## Example Inputs

| Text Input                                            | Output Voice                         |
|-------------------------------------------------------|--------------------------------------|
| Hello! I hope you're having a great day.              | Human-like female voice (LJ Speech)  |
| Wow, that was absolutely amazing!                     | Expressive narration                 |
| Once upon a time, in a land far, far away...          | Storytelling tone                    |

---

## Tools and Libraries Used

- Python  
- Coqui TTS – for speech synthesis  
- Gradio – for user interface  

---

## Planned Features

| Feature             | Description                                            |
|---------------------|--------------------------------------------------------|
| Audio Download      | Allow users to download the generated `.wav` file      |
| Speed Control       | Add option to control speaking speed                   |

---

## Coming Soon

| Feature             | Description                                            |
|---------------------|--------------------------------------------------------|
| Multilingual Support| Support additional languages and accents               |
| Voice Cloning       | Clone a user's voice from a short sample               |
| Custom UI Theme     | Dark mode and advanced UI layout options               |

---
