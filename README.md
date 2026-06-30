# 🎥 AI Meeting Assistant

An AI-powered Meeting Assistant that automatically converts meeting audio or YouTube videos into structured meeting notes.

The application transcribes audio, translates Hindi to English (if needed), generates concise summaries, extracts action items, identifies key decisions, creates professional meeting titles, and exports results as PDF or TXT.

---

## Features

- YouTube video transcription
- Audio file upload support
- Speech-to-Text using Whisper
- Hindi to English translation
- AI-generated meeting summary
- Automatic meeting title generation
- Action item extraction
- Key decision extraction
- Open question detection
- PDF report export
- TXT export
- Streamlit user interface

---

## Tech Stack

### Frontend

- Streamlit

### Backend

- Python

### AI Models

- OpenAI Whisper
- Mistral AI API

### Libraries

- LangChain
- FFmpeg
- yt-dlp
- ReportLab
- Transformers
- Torch

---

## Project Workflow

```text
YouTube URL / Audio File
            │
            ▼
Download Audio
            │
            ▼
Speech-to-Text (Whisper)
            │
            ▼
Translation (Optional)
            │
            ▼
Meeting Summary
            │
            ├── Generate Title
            ├── Action Items
            ├── Key Decisions
            ├── Open Questions
            │
            ▼
Export PDF / TXT
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/video-agent.git
```

Move to the project folder

```bash
cd video-agent
```

Create a virtual environment

```bash
python -m venv .venv
```

Activate the environment

Windows

```bash
.venv\Scripts\activate
```

Linux / macOS

```bash
source .venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file

```env
MISTRAL_API_KEY=your_api_key
SARVAM_API_KEY=your_api_key
```

---

## Run the Application

```bash
streamlit run app.py
```

---

## Screenshots

### Home Page

![Home](assets/home.png)

### Upload Page

![Upload](assets/upload.png)

### Generated Summary

![Summary](assets/summary.png)

---

## Folder Structure

```text
core/
│
├── transcriber.py
├── summarize.py
├── extractor.py
├── translator.py
└── youtube.py
```

---

## Future Improvements

- Speaker diarization
- Multi-language support
- RAG-based meeting search
- Meeting chatbot
- Cloud deployment
- Meeting history database

---

## Author

**Brajpal Singh**

GitHub:
https://github.com/yourusername

LinkedIn:
https://linkedin.com/in/yourprofile

---

## License

MIT License