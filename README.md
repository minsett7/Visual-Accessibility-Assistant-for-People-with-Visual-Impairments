# Visual Accessibility Assistant for People with Visual Impairments

An AI-powered assistant that helps visually impaired individuals navigate their surroundings using computer vision, speech recognition, and large language models.

## Overview

This project is designed to make everyday navigation easier for people with visual impairments.
The assistant combines object detection, speech-to-text, text-to-speech, and a large language model (LLM) to provide real-time guidance about the environment.

Users can:

- Ask questions about their surroundings using voice.
- Get intelligent, context-aware answers about obstacles, people, and objects.
- Hear the response instantly via audio output.   

## System Flow

1. User Input: Voice or image (camera capture).
2. Speech-to-Text (STT): Converts spoken question into text.
3. Object Detection: Identifies objects in the scene using YOLOv8.
4. LLM + Knowledge Base: Answers user’s question with reasoning.
5. Text-to-Speech (TTS): Converts answer into speech for the user.

## Features

- Real-time object detection with YOLOv8.
- Speech recognition for hands-free interaction.
- Conversational responses using LLaMA (via Groq API).
- Voice output for accessibility.
- Modular design (each component can be improved separately).

## Tech Stack  

| Component         | Tool / Library                          |  
|------------------|------------------------------------------|  
| Object Detection | YOLOv8 (Ultralytics)                     |  
| LLM              | LLaMA 3.1 (via Groq API)                 |  
| Speech-to-Text   | OpenAI Whisper / Google Speech API        |  
| Text-to-Speech   | gTTS / pyttsx3                           |  
| Backend          | Flask / FastAPI                          |  
| Frontend         | Tkinter (Desktop) / Flutter (Mobile)     |  

## Installation

1. Clone the repo:

```bash
git clone https://github.com/minsett7/Visual-Accessibility-Assistant-for-People-with-Visual-Impairments.git
cd Visual-Accessibility-Assistant-for-People-with-Visual-Impairments
```

2. Create a virtual environment & install dependencies:

```bash
python -m venv venv
source venv/bin/activate    # On Linux/Mac
venv\Scripts\activate       # On Windows
pip install -r requirements.txt
```

3. Run the application:

```bash
python app.py
```

## Usage

```bash
Visual-Accessibility-Assistant-for-People-with-Visual-Impairments
┣ 📜 app.py # Main application entry point
┣ 📜 ask_groq.py # LLM integration (Groq / LLaMA API)
┣ 📜 audio_tts.py # Text-to-Speech module
┣ 📜 camera_loop.py # Handles camera input loop
┣ 📜 config.py # Configuration settings
┣ 📜 distance.py # Distance calculation logic
┣ 📜 gui.py # GUI interface for desktop
┣ 📜 hazard.py # Hazard detection logic
┣ 📜 proximity.py # Proximity detection logic
┣ 📜 questions.txt # Sample user questions
┣ 📜 scene.py # Scene description module
┣ 📜 stt_recorder.py # Speech-to-Text recorder
┣ 📜 utils_coco.py # Utility functions for COCO dataset labels
┣ 📜 yolov8n.pt # Pretrained YOLOv8 model weights
┗ 📜 README.md # Project documentation
```
