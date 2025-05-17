# 🤖 LangChain – Chat With Your Data
This project leverages LangChain, OpenAI, and vector databases (like Chroma) to allow natural language querying over your own documents and data. It's a foundational implementation of building an AI chatbot that understands your data.

## 🚀 Features
💬 Chat with PDF, TXT, or CSV files using natural language

🧠 Uses LangChain to manage LLM-driven pipelines

🗃️ Supports ChromaDB vector storage

🔗 Integrated with OpenAI’s GPT models

📝 Text embedding for contextual understanding

⚙️ Modular and extensible Python backend

## 🛠️ Tech Stack
Language: Python 3.9+

Core Libraries: LangChain, OpenAI, Chroma, PyPDF2, tiktoken

LLM Provider: OpenAI GPT-3.5 / GPT-4

## 📂 Folder Structure

/langchain-chat-with-your-data

│── main.py                   # Entry point

│── ingest.py                 # Handles data ingestion and vector store creation

│── chat.py                   # Handles querying and chatbot interaction

│── config.py                 # Environment configuration

│── requirements.txt

│── README.md

## 🔧 Setup Instructions

### 1️⃣ Clone the Repository

git clone https://github.com/abhinav744/langchain-chat-with-your-data.git

cd langchain-chat-with-your-data

### 2️⃣ Create and Activate a Virtual Environment

python -m venv venv

source venv/bin/activate        # On Windows: venv\Scripts\activate

### 3️⃣ Install Dependencies

pip install -r requirements.txt

### 4️⃣ Set Up Environment Variables

Create a .env file in the root directory and add:


OPENAI_API_KEY=your_openai_api_key

### 5️⃣ Ingest Your Data

python ingest.py

This script will read documents from the ./data/ folder and generate a vector index.

### 6️⃣ Start Chat Interface

python chat.py

Then enter a query like:


> What is this document about?

## 📁 Data Formats Supported

✅ .pdf

✅ .txt

✅ .csv

(More formats can be added with minor code changes)

## 📈 Use Cases

Internal document search

Customer support knowledge base

Academic paper summarization

Business report querying

## 🔐 Security & Privacy

Your documents are processed locally, and embeddings are stored in a local vector DB (unless configured for cloud). You have full control over your data.


## 🤝 Contributing
Pull requests are welcome! Feel free to fork the repo and submit changes to improve the project.
