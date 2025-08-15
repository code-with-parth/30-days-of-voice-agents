<div align="center">

# 🔮  Aether Voice: Your AI Conversational Partner

**An intelligent, voice-driven AI assistant that listens, understands, and responds in a natural, human-like voice.**
<br/>
*Built for the [30 Days of AI Voice Agents Challenge by Murf AI](https://murf.ai/30days/)*

</div>

---

<div align="center">

![Aether Voice Demo](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExaHd1bmJldG1pMHUwcWtpNWJxdmRld3R4eGVjZ3JhbmJnM2VwaWVvayZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/PxSFAnuubLkSA/giphy.gif)

</div>

---

## ✨ Core Features

* **🗣️ End-to-End Voice Interaction:** From your voice to the AI's and back again, the entire conversation is spoken.
* **🧠 Context-Aware Memory:** Aether remembers the flow of your conversation, allowing for natural follow-up questions.
* **🎨 Dynamic Voice Selection:** Choose from a list of high-quality, realistic AI voices from **Murf AI**.
* **🎤 Real-time Voice Visualizer:** A pulsing animation provides visual feedback while you speak.
* **🛡️ Robust Error Handling:** The agent gracefully handles API failures without crashing, informing the user with a spoken message.
* **✨ Sleek, Minimalist UI:** A clean, modern interface focused entirely on the conversation.

---

## 🛠️ Tech Stack

* **Frontend:** `HTML`, `JavaScript`, `Tailwind CSS`
* **Backend:** `Python`, `FastAPI`, `Uvicorn`
* **Speech-to-Text:** **AssemblyAI**
* **Language Model:** **Google Gemini**
* **Text-to-Speech:** **Murf AI**

---

## 📂 Project Structure

```
.
├── services/
│   ├── stt.py
│   ├── llm.py
│   └── tts.py
├── static/
│   ├── script.js
│   └── error.mp3
├── templates/
│   └── index.html
├── .env
├── app.py
├── README.md
├── requirements.txt
└── schemas.py
```

---

## ⚙️ Getting Started

To run Aether Voice on your local machine, follow these steps.

### **1. Prerequisites**

* Python 3.8+
* An API key for [AssemblyAI](https://www.assemblyai.com/)
* An API key for [Google AI Studio (Gemini)](https://aistudio.google.com/)
* An API key for [Murf AI](https://murf.ai/)

### **2. Clone & Install**

```bash
# Clone the repository
git clone [https://github.com/code-with-parth/30-days-of-voice-agents.git](https://github.com/code-with-parth/30-days-of-voice-agents.git)
cd 30-days-of-voice-agents

# Install the required dependencies
pip install -r requirements.txt
```

### **3. Configure Environment**

Create a `.env` file in the root of the project and add your API keys:

```env
ASSEMBLYAI_API_KEY="your_assemblyai_api_key"
GEMINI_API_KEY="your_gemini_api_key"
MURF_API_KEY="your_murf_api_key"
```

### **4. Launch the Server**

```bash
uvicorn app:app --reload
```

The server will start on `http://127.0.0.1:8000`. Open this URL in your browser to start talking to Aether!

---

<details>
<summary>🏆 <strong>Click here to see my 30-Day Challenge Journey & Daily Log</strong></summary>

## ✅ Day 1:
I built a basic FastAPI web app that allows users to enter a prompt and get a dummy response (simulating a voice agent backend).

🔗 LinkedIn Post: [Day 1 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-buildwithmurf-activity-7357412374795972608-4mYm?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 2:
Created a REST API endpoint to handle text-to-speech requests. This involved setting up a secure way to handle API keys with a `.env` file and calling the Murf AI API to generate audio.

🔗 LinkedIn Post: [Day 2 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-murfai-fastapi-activity-7357713045168578560-Zq-G?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 3:
Built the frontend user interface and connected it to the backend. Used JavaScript's `fetch` API to send user input to the server and then dynamically created an HTML `<audio>` element to play the returned audio.

🔗 LinkedIn Post: [Day 3 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_voiceagents-tts-fastapi-activity-7358171941578399745-f5IN?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 4:
Built a client-side "Echo Bot" using the browser's native `MediaRecorder` API. This feature allows the user to record audio from their microphone and play it back instantly without any server interaction.

🔗 LinkedIn Post: [Day 4 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-30daysofvoiceagents-echobot-activity-7358430121428480000-G8tz?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 5:
Implemented client-to-server audio uploading. The recorded audio is now sent from the browser to a new FastAPI endpoint on the server, which saves the file and returns its metadata.

🔗 LinkedIn Post: [Day 5 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-buildwithmurf-30daysofvoiceagents-activity-7358795264603688961-vOiz?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 6:
Integrated AssemblyAI for speech-to-text transcription. The app now understands spoken words! Also, I gave the entire user interface a major visual overhaul with a new futuristic, "glassmorphism" design.

🔗 LinkedIn Post: [Day 6 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-murfai-assemblyai-activity-7359105732400558080-52UG?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 7 & Bonus Feature:
Completed the Echo Bot v2, which transcribes user audio with AssemblyAI and generates a new response in an AI voice using the **Murf AI** API. I also added a **bonus voice selection feature**, allowing users to choose from a list of dynamically fetched voices.

🔗 LinkedIn Post: [Day 7 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofaivoiceagents-buildwithmurf-activity-7359558682956775424-AQxR?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 8:
Integrated a Large Language Model (LLM) into the backend. I created a new endpoint that sends a user's text query to the Google Gemini API and returns the intelligent, human-like response.

🔗 LinkedIn Post: [Day 8 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-buildwithmurf-ai-activity-7359895688136081408-hUsx?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 9:
Built the full, end-to-end conversational pipeline. The application now listens to a user's voice (AssemblyAI), thinks of a response (Google Gemini), and speaks that response back in a realistic AI voice using the **Murf AI** API.

🔗 LinkedIn Post: [Day 9 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-buildwithmurf-30daysofvoiceagents-activity-7360278126804840448-P4fA?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 10:
Implemented chat history, allowing the AI to remember the context of the conversation. I also added an auto-record feature, which creates a seamless and natural conversational flow.

🔗 LinkedIn Post: [Day 10 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-buildwithmurf-30daysofvoiceagents-activity-7360645789557178368-W6Dk?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 11:
Made the application more robust by adding full-stack error handling. The backend now uses `try...except` blocks to catch API failures and serves a fallback audio file, while the frontend gracefully handles the error state.

🔗 LinkedIn Post: [Day 11 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagent-buildwithmurf-google-activity-7361035992339820544-5Nfy?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 12:
Revamped the user interface for a cleaner, more focused experience. Removed the old UI components and combined the recording buttons into a single, stateful button. Also added a conversation log to display both the user's transcribed text and the AI's response.

🔗 LinkedIn Post: [Day 12 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-buildwithmurf-30daysofvoiceagents-activity-7361358121761484800-XH7R?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 13:
Created a professional `README.md` for the project. The documentation includes a project overview, core features, tech stack, project structure, and detailed setup instructions.

🔗 LinkedIn Post: [Day 13 LinkedIn Post](https://www.linkedin.com/posts/parth-d-720584256_30daysofvoiceagents-buildwithmurf-30daysofvoiceagents-activity-7361686861259464704-aZfi?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD8WwwgB5_T7WEyTmnyEyLnhNMhBXwDVZkM)

## ✅ Day 14:
Refactored the entire backend into a professional, service-oriented architecture. Separated logic for STT, LLM, and TTS into their own modules, added Pydantic schemas for data validation, and implemented a proper logging system. Successfully integrated the Murf AI API for text-to-speech.

🔗 LinkedIn Post: [Day 14 LinkedIn Post]()

</details>
