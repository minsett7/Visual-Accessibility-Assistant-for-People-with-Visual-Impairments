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

- User Input: Voice or image (camera capture).
- Speech-to-Text (STT): Converts spoken question into text.
- Object Detection: Identifies objects in the scene using YOLOv8.
- LLM + Knowledge Base: Answers user’s question with reasoning.
- Text-to-Speech (TTS): Converts answer into speech for the user.

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

Clone the repo:

```bash
git clone https://github.com/minsett7/Visual-Accessibility-Assistant-for-People-with-Visual-Impairments.git
cd Visual-Accessibility-Assistant-for-People-with-Visual-Impairments
```