# Generative AI Question-Answering Bot  

## Overview  
This project is a Generative AI-powered Question-Answering Bot developed using the **LangChain** framework and **GPT-4.0**. The bot dynamically retrieves relevant information from a preprocessed dataset and provides accurate, context-aware responses to user queries.  

## Features  
- **Data Scraping**: Utilized **WebBaseLoader** with **BeautifulSoup** for extracting website data.  
- **Data Processing**: Split the scraped content into manageable chunks using **Recursive Character TextSplitter**.  
- **Vector Embedding**: Converted chunks into vector embeddings stored in a **FAISS vector database**.  
- **Dynamic Retrieval**: Implemented a **retrieval chain** to fetch the most relevant documents based on user queries.  
- **Generative AI**: Powered by **GPT-4.0** for natural language understanding and response generation.  

## Workflow  
1. **Data Ingestion**:  
   - Scrape website data using **WebBaseLoader** with **BeautifulSoup** as the backend.  
   - Preprocess the data into smaller chunks using **Recursive Character TextSplitter**.  

2. **Embedding and Storage**:  
   - Transform text chunks into vector embeddings.  
   - Store embeddings in a **FAISS vector database** for efficient retrieval.  

3. **Retrieval and Question Answering**:  
   - Convert the vector store to a retriever.  
   - Use the **retrieval chain** to dynamically select relevant documents.  
   - Generate responses with **retrievalChain.invoke()**, passing the retrieved context to **GPT-4.0**.  

## Technologies Used  
- **LangChain Framework**  
- **GPT-4.0**  
- **FAISS Vector Database**  
- **BeautifulSoup**  
- **Python**  


