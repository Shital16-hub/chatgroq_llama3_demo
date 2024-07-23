# Chatgroq With Llama3 Demo

This project demonstrates a question-answering system using Groq's Llama3 model and document embeddings. It uses Streamlit for the user interface, allowing users to ask questions about loaded documents.

## Features

- Document embedding using Ollama Embeddings
- Vector storage using FAISS
- Question answering using Groq's Llama3-8b-8192 model
- Streamlit interface for user interaction

## Prerequisites

- Python 3.7+
- Groq API key
- Ollama installed and running locally

## Installation

1. Clone this repository:

2. Install the required packages:

3. Create a `.env` file in the root directory and add your Groq API key:

## Usage

1. Place your PDF documents in the `./us_census` directory.

2. Run the Streamlit app:

3. In the Streamlit interface:
- Click the "Documents Embedding" button to process and embed the documents.
- Once the embedding is complete, enter your question in the text input field.
- The app will display the answer based on the document content.

## How it works

1. The app loads PDF documents from the specified directory.
2. Documents are split into chunks and embedded using Ollama Embeddings.
3. Embeddings are stored in a FAISS vector database for efficient retrieval.
4. User questions are processed using the Groq Llama3 model.
5. Relevant document chunks are retrieved and used to generate an answer.

## Note

Ensure that you have sufficient resources to run the embedding process and the Llama3 model. The current implementation limits processing to the first 20 documents to manage resource usage.

## License

[Specify your license here]
