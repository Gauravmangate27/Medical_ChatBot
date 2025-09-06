# Medical ChatBot

A conversational AI assistant for medical queries, built with Python, LangChain, Pinecone, and Gemini (Google Generative AI). The bot can extract and answer questions from medical PDFs using advanced language models and vector search.

## Features

- Extracts and processes medical information from PDF files
- Splits documents into text chunks for efficient retrieval
- Embeds text using HuggingFace models
- Stores and searches embeddings with Pinecone
- Answers questions using Gemini (Google Generative AI) via LangChain
- Flask web interface with a modern chat UI

## Setup

### 1. Clone the repository

```powershell
git clone https://github.com/Gauravmangate27/Medical_ChatBot.git
cd Medical_ChatBot
```

### 2. Create and activate a virtual environment

```powershell
python -m venv medibot
.\medibot\Scripts\Activate
```

### 3. Install dependencies

```powershell
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Set up environment variables

- Create a `.env` file in the project root.
- Add your API keys (e.g., for Pinecone and Gemini):

```
PINECONE_API_KEY=your-pinecone-api-key
GOOGLE_API_KEY=your-gemini-api-key
```

### 5. Add your PDF files

Place your medical PDF files in the `Data` or `data` directory.

## Usage

- Run the Flask app or Jupyter notebook as needed.
- Example notebook: `research/trials.ipynb`
- The chatbot will process your PDFs and answer medical questions.

## File Structure

- `requirements.txt` — Python dependencies
- `static/style.css` — Chat UI styles
- `research/trials.ipynb` — Main notebook for data processing and Q&A
- `Data/` or `data/` — Directory for your PDF files

## Acknowledgements

- [LangChain](https://github.com/langchain-ai/langchain)
- [Pinecone](https://www.pinecone.io/)
- [Google Generative AI (Gemini)](https://ai.google.dev/)
- [HuggingFace Transformers](https://huggingface.co/)

---

> **Note:** This project is for educational purposes. It is not intended for use as a substitute for professional medical advice.
