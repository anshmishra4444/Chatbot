LangGraph Chatbot with Streamlit
https://demo.gif <!-- Add a demo GIF if available -->

📌 Overview
A conversational AI chatbot built using:

LangGraph for stateful conversation management

LangChain for LLM orchestration

Streamlit for the interactive web interface

The application features:

Multiple conversation threads management

Streaming responses

Persistent chat history

Simple and intuitive UI

🚀 Features
Multi-threaded Conversations: Create and switch between different chat threads

Real-time Streaming: Get responses as they're generated

State Persistence: Conversations are maintained using LangGraph's state management

Simple Interface: Clean Streamlit UI with sidebar navigation

🛠️ Installation
Clone the repository:

bash
git clone https://github.com/yourusername/langgraph-chatbot.git
cd langgraph-chatbot
Set up a virtual environment (recommended):

bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install dependencies:

bash
pip install -r requirements.txt
Create a .env file with your OpenAI API key:

env
OPENAI_API_KEY=your-api-key-here
🏃‍♂️ Running the Application
Choose one of the frontend implementations to run:

Basic Chat Interface
bash
streamlit run streamlit_frontend.py
Streaming Response Interface
bash
streamlit run streamlit_frontend_streaming.py
Threaded Conversation Interface (Recommended)
bash
streamlit run streamlit_frontend_threading.py
🧩 File Structure
text
.
├── langgraph_backend.py       # Core chatbot logic with LangGraph
├── streamlit_frontend.py      # Basic chat interface
├── streamlit_frontend_streaming.py  # Streaming response version
├── streamlit_frontend_threading.py  # Multi-thread conversation version
├── requirements.txt           # Python dependencies
└── .env.example               # Environment variables template
🤖 How It Works
Backend (langgraph_backend.py):

Defines the conversation state using ChatState

Implements a simple chat node with OpenAI

Uses InMemorySaver for conversation checkpoints

Frontend:

streamlit_frontend.py: Basic chat interface

streamlit_frontend_streaming.py: Adds streaming responses

streamlit_frontend_threading.py: Full-featured version with conversation threads

📝 Requirements
Python 3.8+

Streamlit

LangChain

LangGraph

OpenAI API key

python-dotenv

🤝 Contributing
Contributions are welcome! Please open an issue or submit a pull request.
