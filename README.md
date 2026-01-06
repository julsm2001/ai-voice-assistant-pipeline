# 🎙️ Cloud-Based Voice Assistant: STT-LLM-TTS Pipeline

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/julsm2001/ai-voice-assistant-pipeline/blob/main/Voice_Assistant_Pipeline.ipynb)
![Status](https://img.shields.io/badge/Status-Prototype-green)

**Author:** Julián Machuca Ramírez
**Field:** AI Technologist Student & Licensed Music Producer
**Updated:** December 2025

## 🚀 Project Overview
This repository showcases an **End-to-End Voice Interaction System** optimized for cloud environments. Leveraging my background in **Music Production**, I designed this pipeline to handle the complexities of audio-to-text-to-speech workflows using State-of-the-Art (SOTA) AI models with near-zero latency.

### 🧠 Core Technologies
1. **ASR (Automatic Speech Recognition):** `OpenAI Whisper` for robust audio transcription.
2. **LLM (Large Language Model):** `Llama 3.3 (70B)` via **Groq API** for high-speed, intelligent reasoning.
3. **TTS (Text-to-Speech):** `gTTS` for reliable and natural vocal synthesis.

## ⚙️ Architecture & Data Flow
The system implements a seamless sequential pipeline:
**Audio Input** → `OpenAI Whisper` (Transcription) → `Llama 3.3` (Inference) → `gTTS` (Synthesis) → **Audio Output**.

## 🛠️ Key Technical Highlights
* **Advanced Web Integration:** Engineered a custom **JavaScript bridge** to overcome Google Colab's browser-kernel isolation, enabling direct microphone access for cloud-based recording.
* **Latency Engineering:** Integrated **Groq's LPU acceleration**, reducing inference time for the 70B parameter model to near-real-time levels.
* **Signal Awareness:** Designed with an understanding of audio signal processing, ensuring high-fidelity ingestion for the ASR stage.

## 📖 How to Use
1. **Open the Notebook:** Click the "Open in Colab" badge above.
2. **Configure API:** Obtain a free [Groq API Key](https://console.groq.com/keys).
3. **Run Sequentially:** The notebook automates the setup for `ffmpeg`, `pydub`, and all necessary AI dependencies.

---
*Developed as a core project for the AI Technologist Portfolio, bridging technical IT support with advanced Generative AI.*
