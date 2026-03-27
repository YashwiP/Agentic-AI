# Autonomous Research Agent using LangChain
Overview

This project implements an Autonomous Research Agent using LangChain and Google Gemini API. The agent is capable of automatically researching a given topic, extracting key insights, and generating a structured report without human intervention.

The system combines Large Language Models (LLMs) with external tools like web search and Wikipedia to simulate intelligent research behavior.

🎯 Objective

To build an AI agent that can:

Search information from the web
Analyze and summarize data
Generate a structured research report
🚀 Features
🔍 Automated web research using DuckDuckGo
📚 Knowledge retrieval from Wikipedia
🧠 Intelligent reasoning using Gemini LLM
🧾 Structured report generation
⚡ Tool-calling agent (ReAct-style reasoning)
💾 Saves output reports as text files
🛠️ Technologies Used
Python
LangChain
Google Gemini API (gemini-1.5-flash)
DuckDuckGo Search
Wikipedia API
🧩 System Architecture
User Input
→ Topic provided by user
LLM (Gemini)
→ Processes and understands query
Tools Integration
→ Web Search Tool
→ Wikipedia Tool
Agent (Tool-Calling Agent)
→ Decides which tool to use
→ Retrieves relevant information
Output Generator
→ Produces structured report
🔁 Workflow
User enters a research topic
Agent analyzes the query
Selects appropriate tools
Collects and processes data
Generates a structured report
Saves output to file
📂 Project Structure
Research_Agent.py
Output_1.txt
Output_2.txt
README.md
⚙️ Installation & Setup
1. Install Dependencies
pip install langchain langchain-community langchain-google-genai wikipedia duckduckgo-search
2. Set API Key
import os
os.environ["GOOGLE_API_KEY"] = "your_api_key_here"
▶️ How to Run
python Research_Agent.py
📊 Sample Topics
Impact of AI in Healthcare
Future of Solid-State Batteries in Electric Vehicles
📄 Output Format

The generated report includes:

Cover Page
Title
Introduction
Key Findings
Challenges
Future Scope
Conclusion
🧠 Agent Type

This project uses a Tool-Calling Agent in LangChain, which follows a ReAct-style reasoning approach:

Think → Decide → Act (use tools) → Respond
📌 Sample Outputs
Output_1.txt → AI in Healthcare
Output_2.txt → Solid-State Batteries
⚠️ Limitations
Depends on external APIs
May produce slightly varying results
Requires internet access
🔮 Future Improvements
Add Streamlit UI
Export reports as PDF
Add more tools (Arxiv, News APIs)
Improve citation and referencing
✅ Conclusion

This project demonstrates how AI agents can automate the research process by combining reasoning capabilities with external knowledge tools. It highlights the potential of agent-based systems in real-world applications like research, analysis, and report generation.

👨‍💻 Author

YP

📜 License

This project is for academic purposes.
