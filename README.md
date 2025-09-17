# VidChat

VidChat is an AI-powered application that allows you to summarize YouTube videos and ask questions about their content. It leverages state-of-the-art models for speech-to-text, summarization, and question answering, making it a powerful tool for extracting insights from video content.

## Features
- **Summarize YouTube Videos:** Automatically transcribe and summarize the content of any YouTube video.
- **Ask Questions:** Query the summarized content to get answers about specific topics discussed in the video.
- **Embeddings & Search:** Uses embeddings to enable semantic search and context-aware Q&A.

## How It Works
1. **Download Audio:** Extracts audio from a YouTube video using `yt-dlp`.
2. **Transcribe Audio:** Converts audio to text using OpenAI Whisper.
3. **Summarize Content:** Summarizes the transcript using a transformer-based model (BART).
4. **Generate Embeddings:** Creates embeddings for semantic search and Q&A using HuggingFace models and LangChain.
5. **Question Answering:** Uses Gemini LLM to answer questions based on the video content.

## Requirements
- Python 3.8+
- [yt-dlp](https://github.com/yt-dlp/yt-dlp)
- [openai-whisper](https://github.com/openai/whisper)
- [ffmpeg](https://ffmpeg.org/)
- [langchain](https://github.com/hwchase17/langchain)
- [transformers](https://github.com/huggingface/transformers)
- [sentence-transformers](https://www.sbert.net/)
- [google-generativeai](https://github.com/google/generative-ai-python)

## Setup
1. Clone the repository.
2. Install the required Python packages:
	```bash
	pip install yt-dlp openai-whisper ffmpeg-python langchain langchain-huggingface sentence-transformers langchain-chroma langchain-community langchain-openai google-generativeai transformers
	```
3. Obtain your Gemini API key and set it in your environment or code.

## Usage
- Run the `chatyt.py` script and follow the prompts to input a YouTube video URL and your Gemini API key.
- The application will download, transcribe, summarize, and allow you to ask questions about the video content.

## Example
```
python chatyt.py
# Enter YouTube URL and Gemini API Key when prompted
```

## Project Structure
- `chatyt.py` - Main script containing all core logic.
- `ChatYT.ipynb` - Jupyter notebook version for interactive use.

## Author
Achyut Pandey

---
This project is ideal for showcasing on your resume as it demonstrates skills in AI, NLP, LLMs, and end-to-end application development.
