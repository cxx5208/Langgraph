# Langgraph

Langgraph is a cutting-edge platform integrating advanced language models (LLMs) and tools to build and deploy multi-agent systems with Retrieval-Augmented Generation (RAG) workflows. The primary goal of this project is to enable the creation of chatbot architectures that utilize tools like AstraDB and Llama to enhance information retrieval and response generation.

## Key Features
- **Multi-Agent Systems**: Easily build complex systems with multiple agents working together on tasks.
- **Retrieval-Augmented Generation (RAG)**: Augment LLMs with powerful vector store-backed retrieval (AstraDB, Llama) for context-aware, relevant responses.
- **Integration with Tools**: Extend chatbot functionalities by integrating tool invocations, such as Wikipedia searches and database queries.
- **Real-World Use Cases**: End-to-end examples for building LLM-powered applications, including data retrieval, query routing, and generation.

## Usage Overview

The Langgraph repository provides a set of detailed Jupyter notebooks that walk you through different levels of chatbot implementations. Here's how you can use the provided notebooks:

1. **Basic Chatbot Example**: Start with the `1.Chatbot_with_langgraph.ipynb` notebook to understand the foundations of using Langgraph to build a chatbot. This notebook explains the core logic behind question routing and basic LLM interaction.

2. **Tool Integration**: Dive deeper with the `2.Langgraph_Chatbot_with_Tools.ipynb` notebook, which demonstrates how to enhance your chatbot by integrating external tools like Wikipedia for knowledge retrieval. You'll learn how to extend agent capabilities beyond just LLM outputs.

3. **Advanced End-to-End Workflow**: Explore the most comprehensive example in the `3.End_to_End_Multi_AI_Agents_RAG_with_LangGraph_AstraDB_and_Llama_3_1.ipynb` notebook. Here, you will work through building an advanced RAG system powered by AstraDB as the vector store and Llama 3.1 as the language model. This notebook also includes guidance on scaling agents, managing data retrieval, and optimizing query throughput.

---

## Key Components

### 1. **Langgraph**:
   - **Langchain Integration**: Langchain serves as the primary framework for orchestrating LLMs, tools, and agent behaviors.
   - **Question Routing**: Questions are routed between retrieval and wiki search based on the source of the question.

### 2. **AstraDB (Vector Store)**:
   AstraDB plays a central role in handling vector-based data retrieval for augmenting the LLM’s responses. You can view the key metrics of AstraDB's performance in the image below:
   ![Screenshot 2024-09-11 at 1 38 06 AM](https://github.com/user-attachments/assets/c2343e74-ac49-407c-b7b9-271666dc851c)

   This integration allows your chatbot to retrieve relevant information from external datasets, improving the quality of responses.

   **Key Metrics Tracked**:
   - Total Latency
   - Read/Write Throughput
   - Average Throughput

### 3. **Llama 3.1**:
   Llama 3.1 is used as the primary LLM for generating responses. It works in conjunction with the vector store to provide context-aware responses, enabling the chatbot to deliver more accurate and relevant information.

---

## Notebooks Overview

### 1. **[Chatbot with Langgraph](https://github.com/cxx5208/Langgraph/blob/main/1.Chatbot_with_langgraph.ipynb)**:
   This notebook introduces the core chatbot system built using Langgraph. The chatbot can handle queries and route them to the appropriate modules based on the question's nature. It sets up basic functionalities, including simple question routing and response generation.

### 2. **[Langgraph Chatbot with Tools](https://github.com/cxx5208/Langgraph/blob/main/2.Langgraph_Chatbot_with_Tools.ipynb)**:
   The focus here is on extending the chatbot’s capabilities by integrating tools like Wikipedia search. The notebook shows how to build a more complex agent that invokes external APIs or tools to fetch data when needed, enhancing the system's versatility.
  
   ![image](https://github.com/user-attachments/assets/1b9200de-3cb5-4103-b7a0-d61aedb38366)

### 3. **[End-to-End Multi AI Agents RAG with LangGraph, AstraDB, and Llama 3.1](https://github.com/cxx5208/Langgraph/blob/main/3.End_to_End_Multi_AI_Agents_RAG_with_LangGraph_AstraDB_and_Llama_3_1.ipynb)**:
   This advanced notebook demonstrates the creation of a full-fledged multi-agent system for RAG workflows. You will learn how to integrate AstraDB for vector storage and retrieval, combined with Llama 3.1, to build a robust chatbot capable of answering complex queries based on external data sources.
  
   ![image](https://github.com/user-attachments/assets/df5045a4-2559-48d4-9f4a-749c80231c4a)


