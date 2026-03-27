# Autonomous Research Agent using LangChain

## Overview
This project implements an **Autonomous Research Agent** using LangChain and Google Gemini API. The agent is capable of automatically researching a given topic, extracting key insights, and generating a structured report without human intervention.

The system combines **Large Language Models (LLMs)** with external tools like web search and Wikipedia to simulate intelligent research behavior.

---

## Objective
To build an AI agent that can:
- Search information from the web  
- Analyze and summarize data  
- Generate a structured research report  

---

## Features
- Automated web research using DuckDuckGo  
- Knowledge retrieval from Wikipedia  
- Intelligent reasoning using Gemini LLM  
- Structured report generation  
- Tool-calling agent (ReAct-style reasoning)  
- Saves output reports as text files  

---

## Technologies Used
- Python
- LangChain
- Google Gemini API (gemini-1.5-flash)
- DuckDuckGo Search
- Wikipedia API

---

## System Architecture

1. User Input  
   → Topic provided by user  

2. LLM (Gemini)  
   → Processes and understands query  

3. Tools Integration  
   → Web Search Tool  
   → Wikipedia Tool  

4. Agent (Tool-Calling Agent)  
   → Decides which tool to use  
   → Retrieves relevant information  

5. Output Generator  
   → Produces structured report  

---

## Workflow
1. User enters a research topic  
2. Agent analyzes the query  
3. Selects appropriate tools  
4. Collects and processes data  
5. Generates a structured report  
6. Saves output to file  

---

## Project Structure
1. Research_Agent.py
2. Output_1.txt
3. Output_2.txt
4. README.md


---

## How to Run

1. Install dependencies:
   pip install langchain langchain-community langchain-google-genai wikipedia duckduckgo-search

2. Set your API key:
   import os
   os.environ["GOOGLE_API_KEY"] = "your_api_key_here"

3. Run the script:
   python Research_Agent.py

---

## Sample Topics
- Impact of AI in Healthcare  
- Future of Solid-State Batteries in Electric Vehicles  

---

## Output Format
The generated report includes:
- Cover Page  
- Title  
- Introduction  
- Key Findings  
- Challenges  
- Future Scope  
- Conclusion  

---

## Agent Type
This project uses a **Tool-Calling Agent** in LangChain, which follows a **ReAct-style reasoning approach**:
- Think → Decide → Act → Respond  

---

## Sample Outputs
- Output_1.txt → AI in Healthcare  
- Output_2.txt → Solid-State Batteries  

---

## Limitations
- Depends on external APIs  
- May produce slightly varying results  
- Requires internet access  

---

## Future Improvements
- Add Streamlit UI  
- Export reports as PDF  
- Add more tools (Arxiv, News APIs)  
- Improve citation and referencing  

---

## Conclusion
This project demonstrates how AI agents can automate the research process by combining reasoning capabilities with external knowledge tools. It highlights the potential of agent-based systems in real-world applications like research, analysis, and report generation.

---

## Author
YP

---

## License
This project is for academic purposes.
