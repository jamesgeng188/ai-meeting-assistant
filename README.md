# AI Meeting Assistant

An **AI-powered scheduling assistant** built with **OpenAI GPT-4** and **Cal.com APIs**.  
It provides a natural-language interface for booking, listing, and canceling meetings, with robust support for time zones, conflict detection, and error handling.

Run the app locally with:

```bash
streamlit run main.py


Project Overview

This project demonstrates how to integrate conversational AI with calendar APIs to create a seamless meeting management experience.

Core Features

✅ Natural language scheduling – create, list, and cancel events with simple prompts

✅ Time zone handling – automatically converts and validates time across regions

✅ Error recovery – gracefully handles API issues with user-friendly messages

✅ Interactive web UI – powered by Streamlit for quick testing and demos

Tech Stack

Python 3.9+

OpenAI GPT-4 API
 (function calling)

Cal.com REST API

Streamlit
 (frontend)

pytz (time zone support)

requests (HTTP requests)


Setup
1. Clone the repository
git clone https://github.com/jamesgeng188/ai-meeting-assistant.git
cd ai-meeting-assistant
2. Create a virtual environment
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
3. Install dependencies
pip install -r requirements.txt
4. Configure environment variables
Create a .env file:
OPENAI_API_KEY=your_openai_api_key
CAL_API_KEY=your_cal_api_key
CAL_USERNAME=your_cal_username




Project Structure
ai-meeting-assistant/
├── cal_api.py          # Cal.com API wrapper
├── functions.py        # OpenAI function definitions
├── main.py             # Streamlit entrypoint
├── openai_chatbot.py   # AI dialogue + orchestration logic
├── requirements.txt    # Dependencies
└── .env.example        # Sample environment file





Usage

Start the Streamlit app:
streamlit run main.py
Then open your browser at http://localhost:8501



Example interactions

Create a meeting

User: Schedule a 30-min meeting tomorrow at 3 PM about the project
Assistant: Sure, please confirm your email address...



List meetings

User: Show me all upcoming events
Assistant: Here are your scheduled meetings...



Cancel a meeting

User: Cancel my 4 PM meeting today
Assistant: The 4 PM meeting has been canceled.


License

MIT License




