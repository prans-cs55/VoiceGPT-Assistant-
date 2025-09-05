# VoiceGPT-Assistant-
🎙️ Voice Assistant

Your personal assistant powered by OpenAI's GPT model and IBM Watson Speech Services (Speech-to-Text & Text-to-Speech).
This project lets you talk to an AI assistant — ask questions, get spoken answers, and interact naturally.

🚀 Features

🎤 Speech-to-Text (STT): Convert your voice into text using IBM Watson.

🤖 AI Assistant: Uses OpenAI GPT to process messages, answer questions, translate, summarize, and more.

🔊 Text-to-Speech (TTS): Converts GPT’s response back into natural-sounding speech.

🌐 Flask Web App: Clean web interface with microphone input and text chat.

🎨 UI Controls: Toggle light/dark mode and select preferred voice.

🛠️ Tech Stack

Backend: Flask (Python)

Frontend: HTML, CSS, JavaScript

AI: OpenAI GPT (via openai library)

Speech Services: IBM Watson STT & TTS (via REST APIs)

Deployment: Docker

📂 Project Structure
chatapp-with-voice-and-openai-outline/
│── server.py          # Flask backend server
│── worker.py          # Handles STT, TTS, and GPT calls
│── templates/
│   └── index.html     # Frontend UI
│── static/            # JS, CSS, assets
│── requirements.txt   # Python dependencies
│── Dockerfile         # Container setup
│── README.md          # Project documentation

⚙️ Installation
1. Clone Repo
git clone https://github.com/your-username/voice-assistant.git
cd voice-assistant

2. Create Virtual Environment (optional but recommended)
python3 -m venv venv
source venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt

4. Run Flask App
python3 server.py


Server will run at 👉 http://0.0.0.0:8000

🐳 Run with Docker

Build and run the container:

docker build -t voice-chatapp-powered-by-openai .
docker run -p 8000:8000 voice-chatapp-powered-by-openai

🎯 Usage

Open browser at http://localhost:8000

🎤 Click the mic to speak, or type your question.

🤖 Assistant replies with both text + audio response.

🔑 Configuration

IBM Watson STT & TTS endpoints (default: CognitiveClass lab endpoints)

https://sn-watson-stt.labs.skills.network/speech-to-text/api/v1/recognize

https://sn-watson-stt.labs.skills.network/text-to-speech/api/v1/synthesize

OpenAI GPT model: gpt-3.5-turbo (can be updated in worker.py)

📌 Future Improvements

Add support for multiple languages

Deploy on cloud (Heroku, GCP, AWS)

Improve UI with conversation history
