# Smart-Clinic-Intake---Autonomous-Voice-AI-Receptionis

This project is a full-stack web application featuring an AI-powered voice receptionist for a medical clinic. It uses the **Gemini 2.0 Flash Multimodal Live API** for real-time, low-latency voice interactions.

## Features
- **Voice-to-Voice AI**: Native multimodal interaction (STT -> LLM -> TTS in one stream).
- **Appointment Management**: Book, check, and cancel appointments via voice.
- **Emergency Detection**: Automatically escalates life-threatening symptoms.
- **Real-time Dashboard**: View and manage appointments in a clean React interface.
- **SQLite Database**: Persistent storage for all clinic data.

## Tech Stack
- **Frontend**: React, Tailwind CSS, Lucide Icons.
- **Backend**: Node.js, Express.
- **Database**: SQLite (via `better-sqlite3`).
- **AI**: Gemini 2.0 Flash (Multimodal Live API).

## Prerequisites
- **Node.js**: Version 18 or higher.
- **Gemini API Key**: Get one from [Google AI Studio](https://aistudio.google.com/).

## Setup Instructions

1. **Clone or Download** the project files into a folder.
2. **Install Dependencies**:
   ```bash
   npm install
   ```
3. **Configure Environment Variables**:
   - Create a `.env` file in the root directory.
   - Add your Gemini API key:
     ```env
     GEMINI_API_KEY=your_api_key_here
     ```
4. **Run the Application**:
   ```bash
   npm run dev
   ```
5. **Access the App**:
   - Open your browser to `http://localhost:3000`.
   - Ensure you grant microphone permissions when prompted.

## Project Structure
- `server.ts`: Express server and Vite middleware.
- `src/db.ts`: SQLite database logic.
- `src/components/VoiceReceptionist.tsx`: Gemini Live API integration and voice UI.
- `src/components/ClinicDashboard.tsx`: Appointment management UI.
- `src/App.tsx`: Main application layout.
