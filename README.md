# 🎙️ Cloud-Based Voice Assistant: STT-LLM-TTS Pipeline

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/julsm2001/ai-voice-assistant-pipeline/blob/main/Voice_Assistant_Pipeline.ipynb)
![Status](https://img.shields.io/badge/Status-Prototype-green)

**Author:** Julián Machuca Ramírez
**Date:** December 2025

## 🚀 Project Overview
This repository contains an **End-to-End Voice Interaction System** developed to run entirely on the cloud using **Google Colab**. The pipeline integrates three distinct State-of-the-Art (SOTA) AI technologies to simulate a natural conversation loop with zero local setup required.

### 🧠 Core Technologies
1.  **ASR (Automatic Speech Recognition):** `OpenAI Whisper` for high-fidelity audio transcription in Spanish.
2.  **LLM (Large Language Model):** `Llama 3.3 (70B)` via **Groq API** for ultra-low latency inference and natural language understanding.
3.  **TTS (Text-to-Speech):** `gTTS` (Google Text-to-Speech) for reliable audio synthesis.

## ⚙️ Architecture Pipeline
The system processes data in a sequential flow:

`[User Audio Input]` $\rightarrow$ **[Whisper ASR]** $\rightarrow$ `[Text Prompt]` $\rightarrow$ **[Llama 3.3]** $\rightarrow$ `[AI Response]` $\rightarrow$ **[gTTS]** $\rightarrow$ `[Audio Output]`

## 🛠️ Installation & Usage
This project is designed to be plug-and-play via Google Colab.

1.  **Open the Notebook:** Click the file `Voice_Assistant_Pipeline.ipynb` above and then the "Open in Colab" badge.
2.  **API Key:** You will need a free [Groq API Key](https://console.groq.com/keys).
3.  **Execution:** Run the cells sequentially. The environment setup cell handles all dependencies (`ffmpeg`, `pydub`, `groq`, `whisper`).

## 📊 Technical Highlights
* **Cloud Audio Capture:** Implemented a custom JavaScript bridge to bypass browser-kernel isolation limitations in Google Colab, allowing direct microphone recording.
* **Latency Optimization:** Utilized Groq's LPU (Language Processing Unit) hardware acceleration to achieve near-instantaneous text generation.
* **Modularity:** The pipeline is segmented into functional blocks (Ingestion, Processing, Synthesis) for easy debugging and scalability.

---
*Developed as part of the Artificial Intelligence Technologist program portfolio.*
