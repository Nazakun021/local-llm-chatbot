# Local Python Chatbot with Local LLM (Ollama & Llama 3)

## Project Description

This project is a command-line chatbot built using Python. It leverages the power of a locally hosted Large Language Model (LLM) accessed via Ollama, specifically using the Llama 3.2 3B model. The chatbot maintains conversation history and a user-friendly terminal interface.

This project was developed as part of the **Phase 2: Tech Article Challenge** for the **SPARCS (Society of Programmers and Refined Computer Scientists)** membership application at the University of the Philippines Mindanao

## Features

**Conversational AI:** Interact with the Llama 3 model running locally.
**Conversation History:** The chatbot remembers previous turns in the current session.
**Local LLM:** Uses Ollama to serve the LLM, ensuring privacy and offline capability.
**Simple Setup:** Requires Python, Ollama, and a few Python packages.

## Technology Stack

**Language:** Python 3.11
**LLM Serving:** Ollama (https://ollama.com/)
**LLM Model:** Llama 3.2 3B 
**Core Logic:** Langchain (`langchain-ollama`, `langchain-core`)

## Setup Instructions

1.  **Install Ollama:**
    * Follow the instructions on https://ollama.com/ to download and install Ollama for your operating system.

2.  **Pull the Llama 3 Model:**
    * Open your terminal and run the following command.
        ```bash
        ollama run llama3.2
        ```
    * Verify the model is available:
        ```bash
        ollama list
        ```

3.  **Install Python Dependencies:**
    * It's recommended to use a virtual environment:
        ```bash
        python3 -m venv chatbot
        “.\chatbot\Scripts\Activate.ps1” if you're on PowerShell.
        ```
    * Install the required packages:
        ```bash
        pip install langchain langchain-ollama ollama 
        ```

## Usage

1.  **Ensure Ollama Service is Running:**
    * Ollama usually runs as a background service after installation. If not, start it manually.

2.  **Run the Chatbot Script:**
    * Make sure your virtual environment is activated (if used).
    * Execute the Python script from your terminal:
        ```bash
        python your_script_name.py
        ```
    * Replace `your_script_name.py` with the actual name of your Python file.

3.  **Interact:**
    * Follow the on-screen prompts. Type your messages and press Enter.
    * Type `exit` to end the conversation.