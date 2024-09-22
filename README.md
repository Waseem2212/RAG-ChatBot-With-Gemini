# RAG-ChatBot-With-Gemini
This Project contains a Chatbot built using LangChain for PDF query handling, FAISS for vector storage, Google Generative AI (Gemini model) for conversational responses, and Streamlit for the web interface. The chatbot can read PDF files, generate text chunks, store them in a vector store, and provide intelligent responses based on user queries.
# Features
- **PDF Processing:** Upload a PDF document, and the app will extract and split its text into manageable chunks.
- **Vector Storage with FAISS:** The text chunks are stored in a FAISS vector database to enable similarity-based retrieval.
- **Generative AI for Responses:** Uses Google Generative AI (Gemini 1.5 Pro) to provide conversational answers based on retrieved content.
- **Real-time Interaction:** User can ask questions related to the PDF, and the app will return concise, relevant answers.
# Technologies Used
- **LangChain:** To manage document loading, text chunking, and retrieval chains.
- **FAISS:** Vector search engine for storing and retrieving text chunks based on similarity.
- **Google Generative AI (Gemini):** The conversational AI engine for generating responses.
- **Streamlit:** Web-based framework for creating interactive UIs.
- **Python:** For all backend functionality.

# Installation
To run this project locally, follow these steps:
1. Clone the repository:
git clone https://github.com/Waseem2212/RAG-ChatBot-With-Gemini

2. Install the dependencies:
pip install -r requirements.txt
3. Set up your API keys:
GOOGLE_API_KEY=your-google-generative-ai-key
4. Run the application:
streamlit run chatbot.py

# Project Structure
📦 rag-application
│

├── chatbot.py            # Main application logic

├── requirements.txt      # Python dependencies

└── README.md             # Project documentation

# How It Works
1. **PDF Loading:** The app uses PyPDFLoader to load and extract text from a provided PDF.

2. **Text Chunking:** The text is split into smaller chunks using RecursiveCharacterTextSplitter for better processing and retrieval.

3. **Vector Storage:** The text chunks are embedded using Google Generative AI embeddings and stored in a FAISS vector store for efficient similarity search.

4. **Question Answering:** When the user asks a question, relevant text chunks are retrieved from the vector store, and Google Generative AI generates a concise answer based on this content.
5. **Real-Time Responses:** The response is displayed in the Streamlit chat interface.



