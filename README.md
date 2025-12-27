# 🎬 Smart YouTube Video Summarizer

An AI-powered web application that automatically extracts transcripts from YouTube videos and generates concise summaries using state-of-the-art Natural Language Processing models.

## 🎯 Overview

Tired of watching lengthy YouTube videos to extract key information? This tool saves you time by:
- Extracting full transcripts from any YouTube video
- Processing and cleaning the text
- Generating intelligent summaries using AI
- Presenting results in a clean, user-friendly interface

**Perfect for:** Students, researchers, content creators, and anyone who wants to quickly understand video content without watching the entire video.

## ✨ Features

- 🚀 **Fast Processing** - Summarize videos in seconds
- 🌍 **Multilingual Support** - Works with English and Arabic transcripts
- 🤖 **AI-Powered** - Uses transformer models for high-quality summaries
- 💻 **User-Friendly Interface** - Clean, intuitive Streamlit web app
- 📱 **Responsive Design** - Works on desktop and mobile devices
- 🔗 **Flexible URL Support** - Accepts both standard and shortened YouTube URLs
- ⚡ **Smart Caching** - Faster performance with intelligent caching
- 🎨 **Clean Output** - Well-formatted, readable summaries


## 🛠️ Tech Stack

### Frontend
- **Streamlit** - Web application framework
- **Python 3.8+** - Core programming language

### AI/ML
- **HuggingFace Transformers** - Pre-trained language models
- **PyTorch** - Deep learning framework
- **DistilBART** - Efficient summarization model (sshleifer/distilbart-cnn-12-6)

### APIs & Libraries
- **YouTube Transcript API** - Transcript extraction
- **SentencePiece** - Tokenization
- **Regular Expressions (re)** - Text processing

### Deployment
- **Streamlit Cloud** - Free cloud hosting
- **Git/GitHub** - Version control


## ⚙️ How It Works

### Architecture Flow

```
┌─────────────────┐
│  YouTube URL    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Extract Video ID│
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Fetch Transcript│ (YouTube Transcript API)
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Clean & Process │ (Text normalization)
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Chunk Text      │ (1024 chars/chunk)
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ AI Summarization│ (DistilBART Model)
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Display Summary │
└─────────────────┘
```

## 📁 Project Structure

```
youtube-summarizer/
│
├── Summarizer.py           # Main application file
├── requirements.txt        # Python dependencies
├── README.md              # Project documentation
├─
```

## ⚙️ Configuration

### Model Configuration

### Supported Languages

Currently configured for:
- English (`en`)
- Arabic (`ar`)


**Made with ❤️ and ☕ by [Muhammed Waheed]**
