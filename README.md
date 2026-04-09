# 🎤 RAG-Based Voice Interview Coach

## 🚀 Overview

The **RAG-Based Voice Interview Coach** is an AI-powered, voice-interactive interview preparation system. It leverages **Retrieval-Augmented Generation (RAG)** and **Agentic AI** to dynamically generate interview questions, evaluate spoken answers, and provide real-time feedback in both text and voice format.

This project simulates a realistic interview environment, helping users practice and improve their communication and technical skills.

## ✨ Features

* 🎙️ **Voice-Based Interaction**

  * Speak your answers using microphone input
  * Converts speech to text using Whisper

* 🧠 **AI-Generated Questions**

  * Dynamically generates domain-specific interview questions
  * Provides model answers for evaluation

* 📊 **Answer Evaluation**

  * Compares user responses with expected answers
  * Gives concise feedback (correctness + improvement tips)

* 🔊 **Text-to-Speech Feedback**

  * Converts feedback into audio using gTTS

* 🔄 **Resilient LLM Integration**

  * Uses OpenRouter API with:

    * Retry logic
    * Model fallback mechanism
    * Auto-discovery of working free models

* 🌐 **Interactive UI**

  * Built with Gradio
  * Real-time audio processing
  * Clean and user-friendly interface

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Core Concepts:** RAG, Agentic AI, LLMs
* **Libraries & Tools:**

  * Whisper (Speech-to-Text)
  * gTTS (Text-to-Speech)
  * Gradio (Frontend UI)
  * OpenRouter API (LLM access)
  * NumPy, Requests, JSON

## 🔄 How It Works

1. **Question Generation**

   * Uses LLM to generate questions + model answers

2. **Voice Input**

   * User speech → Whisper → Text

3. **Evaluation**

   * LLM compares user answer with expected answer

4. **Feedback**

   * Text feedback + Audio output via gTTS

5. **Agentic Flow**

   * Maintains interview state across questions
   * Handles retries and failures gracefully


## 🧠 Key Concepts Used

* **RAG (Retrieval-Augmented Generation):**
  Enhances LLM responses using structured prompts and expected answers.

* **Agentic AI:**
  Manages interview flow, state, and decision-making (next question, evaluation, etc.)

* **Fallback Mechanism:**
  Automatically switches models if one fails.

## ⚠️ Limitations

* Depends on free LLM availability via OpenRouter
* Whisper model may be slower on low-end systems
* Requires stable internet connection

## 🔮 Future Improvements

* Add scoring system and performance analytics
* Store interview history
* Support multiple languages
* Deploy as full-stack web app
* Integrate resume-based question generation

