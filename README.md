PDF Chatbot – AI-Powered Multi-Document Q&A App:

An interactive Streamlit web application that lets users upload multiple PDF files and chat with them using natural language questions.
This app leverages LangChain, FAISS, DeepSeek-Coder-V2 LLM, and HuggingFace Instruct Embeddings to provide intelligent, document-aware responses.

Features:

📚 Upload and chat with multiple PDFs at once

🤖 Ask natural language questions and receive AI-generated answers based strictly on your PDFs

🧠 Maintains conversation history with context using LangChain’s memory

🔍 Uses semantic search (via FAISS) to retrieve the most relevant document chunks

🧩 Powered by DeepSeek-Coder-V2-Lite-Instruct-Q4_K_M.gguf for LLM responses

🌐 Clean and intuitive Streamlit interface

How It Works:

1. Text Extraction: Extracts text from uploaded PDFs using PyPDF2.

2. Text Chunking: Splits the text into manageable chunks using CharacterTextSplitter.

3. Embeddings: Generates embeddings via HuggingFace's hkunlp/instructor-xl.

4. Vector Store: Stores vectors in FAISS for fast and efficient similarity search.

5. LLM Response: Uses DeepSeek-Coder-V2-Lite-Instruct LLM via LlamaCpp to generate contextual answers.

6. Chat Interface: Displays user/AI messages using a custom HTML template with chat memory.

Download the Model:
DeepSeek-Coder-V2-Lite-Instruct-Q4_K_M.gguf

📌 Note
If a question is asked about something not present in the documents, the chatbot will respond:
"That information is not available in the PDF."
All responses are fully grounded in the PDFs you upload.
