# CustomerServiceAgent

An intelligent customer service assistant built with **Streamlit**, **LangChain-style agents**, and **RAG (Retrieval-Augmented Generation)**.  
This project is designed for smart cleaning / robot vacuum scenarios and supports knowledge-based question answering, tool calling, and context-aware response generation.

## Overview

CustomerServiceAgent is a chatbot system that combines a large language model, vector retrieval, and external tools to provide more accurate and practical answers in customer service scenarios.

The project is especially suitable for:

- Product Q&A
- After-sales support
- Knowledge base assistance
- Report-style response generation
- Smart appliance customer service demos

At the current stage, the project is structured around a Streamlit front end, an agent execution layer, and a RAG-based knowledge retrieval pipeline.

---

## Features

### 1. Interactive Chat Interface
- Built with **Streamlit**
- Supports conversational user input
- Displays assistant responses in a chat-style UI
- Streams model output for a smoother interaction experience

### 2. Retrieval-Augmented Generation (RAG)
- Loads local knowledge documents
- Splits and indexes documents into a vector database
- Retrieves relevant content before generating responses
- Improves factual grounding for domain-specific questions

### 3. Agent-Based Tool Calling
The assistant can use multiple tools to answer different types of requests, such as:

- Knowledge base summarization
- Weather lookup
- User location lookup
- User ID retrieval
- Current month retrieval
- External data fetching
- Context filling for report generation

### 4. Prompt Switching
The system supports dynamic prompt behavior for different tasks, including:

- General customer service dialogue
- RAG-based summarization
- Report generation scenarios

### 5. Modular Project Design
The codebase is organized into clear modules for:

- agent logic
- RAG services
- model factory
- prompt templates
- configuration management
- utility functions

This makes the project easier to maintain and extend.

---

## Project Structure

```bash
CustomerServiceAgent/
├── agent/                  # Agent logic, tools, and middleware
├── config/                 # YAML configuration files
├── data/                   # Knowledge base and external data
├── model/                  # Model and embedding factory
├── prompts/                # Prompt templates
├── rag/                    # RAG services and vector store logic
├── utils/                  # Utility modules
├── app.py                  # Streamlit application entry point
└── .gitignore
