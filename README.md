🩺 HealthMaxxer.ai

AI-Powered Healthcare Assistant & Smart Diagnostic Platform

HealthMaxxer.ai is an intelligent healthcare web application built with Flask, LangChain, Gemini, and DeepFace. It provides real-time diagnostics, emotion-aware therapy chat, camera-based interactions, voice input, and emergency contact alerts — all inside a clean, responsive web interface.

🚀 Features
🔍 AI Diagnostic Assistant

Uses LangChain + Gemini Pro to analyze symptoms.

Maintains conversation history using Flask sessions.

Supports camera feed, speech-to-text, and text input.

🧠 Emotion-Aware Therapist Chatbot

Detects facial emotions using DeepFace (webcam snapshot).

Combines emotion history + conversation history to generate empathetic responses.

Provides continuous mental-health support.

🧑‍⚕️ User Accounts

User signup/login using bcrypt for secure hashing.

Each user can add an emergency contact number.

Stores session history and preferences.

📸 Live Camera Processing

Frontend camera preview.

Backend extracts frames for emotion detection and AI context.

🎤 Speech Input

Convert microphone input to text and send it directly to the diagnostic assistant.

🌐 Responsive Design

Fully responsive UI for PC and mobile.

CSS themes with light/dark mode support.

🛠️ Tech Stack
Backend

Flask (Python)

LangChain

Google Gemini Pro (via langchain_google_genai)

DeepFace

SQLite

Frontend

HTML / CSS / JS

Responsive components

Camera & audio APIs

⚙️ Installation & Setup
1️⃣ Clone Repository
git clone https://github.com/yourusername/HealthMaxxer.ai.git
cd HealthMaxxer.ai

2️⃣ Create Virtual Environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Add Environment Variables

Create .env:

GEMINI_API_KEY=your_key_here
SECRET_KEY=your_secret_key

5️⃣ Run Application
flask run

🤖 AI Features Explained
LangChain + Gemini Diagnostic Agent

Takes user text/symptoms.

Adds previous conversation memory.

Optionally includes webcam image descriptions for more context.

Outputs diagnoses, suggestions, and follow-up questions.

DeepFace Emotion Model

Detects:

happy 😄

sad 😢

angry 😠

fear 😨

neutral 😐

surprise 😲

Emotion history influences chatbot tone and responses.

🛡️ Security

Passwords hashed using bcrypt.

Session-based authentication.

API keys stored securely using environment variables.

Camera and microphone usage requires explicit user permission.

📌 Future Enhancements

Realtime vitals analysis using TensorFlow Lite models

Multi-language support

Chat session export to PDF

Emergency SMS alerts
