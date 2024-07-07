# RAG_LLM_BASIC

This project integrates a conversational retrieval system using a combination of large language models (LLMs) and retrieval-augmented generation (RAG) techniques, specifically designed for processing and answering questions based on PDF and text files. It leverages the power of Hugging Face's transformers and custom chainlit (cl) modules to provide an interactive chat experience where users can upload documents and ask questions directly related to the content of those documents.

## Features

- **File Upload**: Users can upload PDF or text files up to 20MB in size.
- **Conversational Interface**: Through an interactive chat, users can ask questions about the uploaded document.
- **Retrieval-Augmented Generation**: Utilizes a combination of LLMs for understanding and generating responses, and RAG for retrieving relevant information from the uploaded document.
- **Source Document Citation**: When providing answers, the system also cites the source documents from the uploaded file.

## How It Works

1. **File Upload**: The system prompts the user to upload a file (PDF or text) upon starting the chat.
2. **File Processing**: Uploaded files are processed to extract text and convert it into a format suitable for retrieval and generation tasks.
3. **Asking Questions**: Users can ask questions related to the content of the uploaded document.
4. **Retrieving Answers**: The system retrieves relevant information from the document and generates a response using a conversational retrieval chain.

## Setup and Installation

This project requires Python 3.6+ and the following libraries:

- `chainlit`
- `torch`
- `transformers`
- `langchain_huggingface`
- `langchain_community`
- `langchain_chroma`
- `langchain_core`

To set up the project, follow these steps:

1. Clone the repository to your local machine.
2. Run the notebook `LLM_RAG_CHAINLIT.ipynb` using Jupyter Notebook or Google Colab to start the application.

## Usage

After setting up the project, follow the instructions in the `LLM_RAG_CHAINLIT.ipynb` notebook to start the chat interface. Upload your document and begin asking questions related to the document's content.