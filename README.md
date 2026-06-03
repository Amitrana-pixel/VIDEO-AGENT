# 🎥 TubeTalk AI

TubeTalk AI is an AI-powered Video Intelligence Platform that transforms YouTube videos and local video files into searchable knowledge.

The application automatically transcribes video content, generates summaries, extracts actionable insights, and allows users to chat with videos using Retrieval-Augmented Generation (RAG).

---

## ✨ Features

### 🎙️ Intelligent Transcription
- English Videos → OpenAI Whisper
- Hinglish Videos → Sarvam AI

### 📝 AI-Powered Summarization
- Concise video summaries
- Topic understanding
- Content condensation

### 🔍 Insight Extraction
- ✅ Action Items
- 🔑 Key Decisions
- ❓ Open Questions

### 🧠 RAG-Based Video Chat
- Ask questions about any video
- Context-aware responses
- Semantic search over video content

### 🎥 Video Support
- YouTube URLs
- Local Video Files
- Audio Files

---

## 🚀 How It Works

### Step 1: Video Input

User provides:

- YouTube URL
- Local video file

### Step 2: Audio Processing

Audio is extracted using:

- yt-dlp
- FFmpeg
- PyDub

### Step 3: Speech-to-Text

TubeTalk AI automatically selects the transcription engine:

#### English Videos

```text
OpenAI Whisper
```

#### Hinglish Videos

```text
Sarvam AI
```

### Step 4: AI Analysis

Transcript is processed using:

```text
LangChain
Mistral AI
```

The system generates:

- Summary
- Action Items
- Key Decisions
- Open Questions

### Step 5: Vector Database Creation

Transcript chunks are converted into embeddings using:

```text
Sentence Transformers
HuggingFace Embeddings
```

Stored in:

```text
ChromaDB
```

### Step 6: Conversational RAG

Users can ask questions such as:

```text
What are the key takeaways?
```

```text
Summarize the video in 5 bullet points.
```

```text
What decisions were made?
```

```text
What action items were discussed?
```

---

## 🛠️ Tech Stack

### Frontend

- Streamlit

### LLM & AI

- Mistral AI
- OpenAI Whisper
- Sarvam AI

### RAG Framework

- LangChain
- LangChain Community
- LangChain Chroma

### Embeddings

- Sentence Transformers
- HuggingFace Embeddings

### Vector Database

- ChromaDB

### Audio Processing

- yt-dlp
- FFmpeg
- PyDub

### Backend

- Python

---

## 📂 Project Structure

```text
TubeTalk-AI/
│
├── core/
│   ├── extractor.py
│   ├── rag_engine.py
│   ├── summarize.py
│   ├── transciber.py
│   └── vector_store.py
│
├── utils/
│   └── audio_processor.py
│
├── app.py
├── main.py
├── requirements.txt
├── .env
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/TubeTalk-AI.git
cd TubeTalk-AI
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Environment

Windows:

```bash
.venv\Scripts\activate
```

Linux / Mac:

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file:

```env
MISTRAL_API_KEY=your_mistral_api_key
SARVAM_API_KEY=your_sarvam_api_key
```

---

## ▶️ Run Application

```bash
streamlit run app.py
```

Open:

```text
http://localhost:8501
```

---

## 💡 Use Cases

- 📚 Educational Videos
- 🎙️ Podcasts
- 🎥 YouTube Content
- 🧑‍🏫 Lectures
- 📺 Webinars
- 🎤 Interviews
- 📖 Online Courses

---

## 🔮 Future Enhancements

- Multi-language support
- Speaker diarization
- PDF report generation
- Cloud storage integration
- Team collaboration features
- Timestamp-based citations

---

## 👨‍💻 Developer

### Amit Kumar Rana 🚀

Built with:
- Python
- Streamlit
- LangChain
- Mistral AI
- Whisper
- Sarvam AI
- ChromaDB

---

## ⭐ If you like this project

Give it a star on GitHub and feel free to contribute!
