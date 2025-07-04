# 🎓 EduTrack LangGraph

EduTrack LangGraph is an AI-powered multi-agent assistant that uses **LangGraph** and **LangChain** to provide personalized academic, wellness, career, and performance guidance to students.

This project demonstrates how intelligent agent routing, dynamic prompt grounding, and real-time data integration can support students with actionable and contextual responses using CSV datasets.

---

## 🚀 High-Level Goals

- Dynamically classify multi-intent student queries using an LLM-based router.
- Trigger appropriate specialized agents (academic, wellness, career, performance).
- Ground each agent's response with context from relevant datasets (GPA, stress levels, career goals, etc.).
- Log agent flow for traceability and debugging.
- Deliver all responses in under 3 seconds using LangGraph's composable graph execution.

---

## 🛠️ Requirements

- Python 3.9+
- Streamlit
- LangGraph
- LangChain
- `langchain-groq` (for Llama3)
- Pandas

---

## Install all dependencies using:

pip install -r requirements.txt

---

 ## ▶️ How to Run
 
### 1.Clone the repository:

```bash

git clone https://github.com/<your-username>/<your-repo-name>.git

cd <your-repo-name>

```

### 2.Add your Groq API key in edutrack_app.py:

```bash

llm = ChatGroq(

    temperature=0,
    
    model_name="llama3-8b-8192",
    
    api_key="YOUR_GROQ_API_KEY"
    
)

```

### 3.Run the Streamlit app:

```bash

streamlit run edutrack_app.py

```

### 4.Input a sample query like:

```bash

Student ID 1001 is struggling with low GPA and exam scores, feels mentally exhausted, and wants career guidance in tech/design.

```

---

