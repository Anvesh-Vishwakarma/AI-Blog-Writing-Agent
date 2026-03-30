# 🚀 AI Blog Writing Agent (LangGraph + Streamlit)

An advanced AI-powered Blog Writing Agent that automatically generates high-quality, structured, and visually enhanced blogs using LangGraph, LLMs, and real-time research.

![image alt](https://github.com/Anvesh-Vishwakarma/AI-Blog-Writing-Agent/blob/main/Screenshot%202.png?raw=true)

This project demonstrates a multi-agent workflow system capable of:
* Planning blog structure
* Performing research
* Writing sections in parallel
* Generating images
* Producing a complete downloadable blog

# 📌 Features

✅ Multi-Agent Architecture (LangGraph)

* Router → Research → Planner → Workers → Reducer
* Parallel content generation using task fan-out

✅ Smart Research System

* Automatically decides when web research is needed
* Uses Tavily API for real-time information

✅ AI Blog Generation

Structured blog creation with headings, sections, and flow
Supports multiple blog types:
* Explainer
* Tutorial
* News Roundup
* Comparison

✅ Image Generation Pipeline

* Automatically decides where images are needed
* Generates diagrams using Gemini Image API
* Embeds images directly into markdown

✅ Interactive Streamlit Frontend

* Live progress tracking (like ChatGPT streaming)
* Markdown preview with images
* Download options:
* Markdown file
* Full bundle (MD + images)

✅ Past Blog Management

* Load previously generated blogs
* Reuse and edit content

# 🧠 Architecture Overview

![image alt](https://github.com/Anvesh-Vishwakarma/AI-Blog-Writing-Agent/blob/main/Screenshot%203.png?raw=true)

# 🛠️ Tech Stack

* Frontend: Streamlit
* Backend: LangGraph
* LLM: OpenAI (GPT-4.1-mini)
* Research API: Tavily
* Image Generation: Google Gemini
* Data Handling: Pandas
* Environment: Python

# ⚙️ Installation

1️⃣ Clone Repository
```
git clone https://github.com/Anvesh-Vishwakarma/AI-Blog-Writing-Agent.git
cd blog-writing-agent
```

2️⃣ Create Virtual Environment
```
python -m venv venv
source venv/bin/activate  # (Linux/Mac)
venv\Scripts\activate     # (Windows)
```

3️⃣ Install Dependencies
```
pip install -r requirements.txt
```

4️⃣ Setup Environment Variables
* Create a .env file and your openai, google-genai and Tavily API key here:
```
OPEN_API_KEY=your_openai_key
GOOGLE_API_KEY=your_gemini_key
TAVILY_API_KEY=your_tavily_key
```

▶️ Run the Application
```
streamlit run bwa_frontend.py
```

# 💡 How It Works
1. User enters a topic
2. Router decides:
   * Need research or not
3. Research node fetches real-time data
4. Orchestrator creates a structured plan
5. Workers generate sections in parallel
6 Reducer:
   * Merges content
   * Adds images
7. Final blog is generated + downloadable

# 📦 Output

The system generates:

📄 Markdown Blog

🖼️ Images Folder

📦 Downloadable ZIP (Blog + Images)



