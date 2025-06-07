# Youtube ChatBot
````markdown
# 🎥 RAG-based YouTube Video Chatbot

A local Retrieval-Augmented Generation (RAG) chatbot that lets you ask questions about YouTube videos by using their transcripts.

## 🚀 Features

- Query YouTube video content using natural language
- Extracts transcripts and builds a local knowledge base
- RAG pipeline to retrieve relevant chunks before answering
- Works locally with your own GRQ API key

## 🧠 Tech Stack

- Python
- YouTube Transcript API
- GRQ (Generative Retrieval + Completion)
- LangChain (for RAG)
- FAISS  (for vector storage)

## 🛠️ Installation

```bash
git clone https://github.com/Akataruka/YouTube_ChatBot_RAG.git
cd YouTube_ChatBot_RAG
pip install -r requirements.txt
````

## 🔑 Using Your Own GRQ API Key

To use your own GRQ (Generative Retrieval) API key:

1. **Get your API key** from your GRQ provider.
2. **Create a `.env` file** in the project root:

```
GROQ_API_KEY=your_grq_api_key_here
```

3. Alternatively, set it directly in your environment:

```bash
export GROQ_API_KEY=your_grq_api_key_here
```

> ⚠️ Never share or commit your API key to a public repository.

## ▶️ How It Works

1. Extracts the transcript from a YouTube video using the video ID.
2. Chunks the transcript and embeds it using a vector model.
3. Stores chunks in a vector database.
4. For any user query:

   * Retrieves top relevant transcript chunks
   * Feeds them into the GRQ model along with the query
   * Returns a concise, contextual answer

## 🧪 Example Queries

* “What are the key takeaways from this video?”
* “Summarize the steps explained by the speaker.”
* “What was discussed in the last 5 minutes?”

## 🤝 Contributing

Feel free to fork this project and submit pull requests. Issues and feature suggestions are welcome!

## 📄 License

MIT License

```

Let me know if you'd like this tailored for a specific GRQ provider or pipeline tool like LangChain or LlamaIndex.
```
