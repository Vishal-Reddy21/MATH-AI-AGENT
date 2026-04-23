 AI Math Agent with Memory
 Overview

This project is an AI-powered math agent that converts natural language input into mathematical expressions and solves them using symbolic computation.

It combines:

* Natural language understanding (via Gemini)
* Mathematical execution (via SymPy)
* Context awareness (via memory system)
 Features

* ✅ Understands messy human input
* ✅ Converts text → math expressions
* ✅ Solves equations and calculations
* ✅ Supports follow-up queries (memory)
* ✅ Context-aware responses like ChatGPT
 Architecture

User Input → Gemini (LLM) → Clean Expression → SymPy → Result → Memory Update


 Tech Stack

* Python
* Google Gemini API
* SymPy
* Regex


 Project Structure


main.py        # Core AI agent
README.md      # Project documentation




 Setup Instructions

 1. Clone the Repository


git clone https://github.com/your-username/ai-math-agent.git
cd ai-math-agent



 2. Install Dependencies


pip install sympy google-generativeai



 3. Set API Key (IMPORTANT)
Mac/Linux:


export GEMINI_API_KEY="your_api_key_here"


 Windows:


set GEMINI_API_KEY=your_api_key_here




4. Run the Project


python main.py




Example Usage


You: take seven squared and subtract fifty  
Bot: -1  

You: add 10 to that  
Bot: 9  

You: what was the last result  
Bot: Last result was: 9  

Memory System

The agent stores:

* Last result
* Recent conversation history

This enables:

* Follow-up queries
* Context-aware reasoning

 Notes

* Do NOT expose your API key publicly
* Use environment variables for security
* Free-tier Gemini API has rate limits

 Future Improvements

* Multi-user support
* Web interface (Streamlit / React)
* Persistent memory (database)
* Advanced reasoning (multi-step planning)
