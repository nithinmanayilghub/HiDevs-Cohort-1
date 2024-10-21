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
