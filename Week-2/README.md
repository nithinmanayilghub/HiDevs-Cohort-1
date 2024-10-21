# Customer Support Chatbot

Eric is a customer support chatbot designed to efficiently manage ticketing for Voltathena, a fictional e-commerce company specializing in tech products. This intelligent assistant streamlines customer interactions, ensuring timely and effective resolution of inquiries while enhancing the overall shopping experience.

An End-to-End open-source **Conversational AI Chatbot** built to enhance customer service by leveraging NLP, LangChain, and Hugging Face models. This project allows users to build a chatbot that retrieves and interacts with various documents using **Retrieval-Augmented Generation (RAG)** and serves responses through a **Gradio interface**. 

## Techniques Employed

- **Document Parsing and Chunking**: Processes and splits PDFs and text documents for efficient retrieval.
- **Vector Store Integration**: Uses **Chroma** for vector storage to retrieve relevant information.
- **Language Model Support**: Supports **Hugging Face Models** for chat response generation.
- **Conversation Memory**: Tracks chat history using **LangChain's ConversationBufferMemory**.
- **Few-Shot Prompting**: Creates dynamic responses with minimal user input.
- **Easy Deployment**: Deploy via **Gradio** interface with custom themes.

---

## Installation

Before running the chatbot, make sure you have all the necessary packages installed. Use the following commands to set up the environment:

`pip install -r requirements.txt`

## Architecture Overview
The Customer Support Chatbot architecture leverages conversational AI models with a robust retrieval-augmented generation (RAG) pipeline, which ensures responses are accurate and context-aware. Below is an outline of the core components and workflow.

### Architecture Pipeline Summary

#### 1. Document Loading and Preprocessing

Loads PDFs, manuals, and product catalogs from the provided knowledge base.
Splits content into chunks using the CharacterTextSplitter for better indexing.
Non-English texts are filtered out using langdetect.

#### 2. Vectorization and Indexing

Converts processed text into vector embeddings using HuggingFace Embeddings.
Stores embeddings in a Chroma vector database for efficient retrieval.
Retrieval Chain Design

#### 3. Retrieval Chain Design
Uses Conversational Retrieval Chains to query the vector store.
The retriever utilizes Maximal Marginal Relevance (MMR) to return the most relevant documents.

#### 4. Retrieval Chain DesignFew-Shot Prompting

A prompt template is designed to guide responses.
Templates include contextual examples for resolving product-specific issues (e.g., product troubleshooting, refund requests).

#### 5. Model Deployment

The chatbot employs the Zephyr 7B model from HuggingFace for text generation.
Responses are shaped by previous interactions using ConversationBufferMemory.
Chat Interface using Gradio

A Gradio interface enables seamless interaction between users and the chatbot.
The interface runs on a shared public link for easy testing and deployment.

![alt text](https://github.com/nithinmanayilghub/HiDevs-Cohort-1/blob/main/Week-2/Week-2%20Chatbot%20Image.png?raw=true)

## Conclusion
This chatbot architecture ensures quick and context-sensitive responses by leveraging retrieval-augmented generation combined with memory-enhanced conversations. The system is designed for seamless deployment and offers low-cost, high-accuracy performance by utilizing models and vector-based search technologies effectively.
