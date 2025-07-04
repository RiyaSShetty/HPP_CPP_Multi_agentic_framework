# 🎓 EduTrack LangGraph

EduTrack LangGraph is an AI-powered multi-agent assistant that uses LangGraph and LangChain to provide personalized academic, wellness, career, and performance guidance to students.

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

Install all dependencies using:

```bash
pip install -r requirements.txt

▶️ How to Run
Clone the repository:

git clone https://github.com/yourusername/EduTrack-LangGraph.git
cd EduTrack-LangGraph
Add your Groq API key in edutrack_app.py:

python
Copy
Edit
llm = ChatGroq(
    temperature=0,
    model_name="llama3-8b-8192",
    api_key="YOUR_GROQ_API_KEY"
)
Run the Streamlit app:
streamlit run edutrack_app.py

Input a sample query like:
Student ID 1001 is struggling with low GPA and exam scores, feels mentally exhausted, and wants career guidance in tech/design.
📂 Sample Input
File: sample_query.txt


Ankit R, student ID 1001, is scoring low on exams and feels mentally drained. He wants help with improving grades and exploring tech-based career paths.
📸 Screenshots
Input	Agent Flow	Responses

💡 Key Contributions & Learnings
👤 Riya S Shetty

Implemented the entire LangGraph pipeline for multi-agent orchestration.

Designed the agent flow with data grounding using real CSV datasets.

Integrated Streamlit for real-time demo and logging UI.

Discovered how LangGraph’s conditional edge routing and state tracking offer scalability over static chains.

Conducted performance tuning to ensure sub-3 second query responses.

📘 Related Work
This is part of a 3-part comparative study:

✅ LangGraph — This repo

🧠 CrewAI — Managed by Teammate 1

🤖 AutoGen — Managed by Teammate 2

All implementations will be merged under a unified GitHub organization repo once complete.

📄 License
MIT License (add LICENSE file if required).

🙌 Acknowledgements
Thanks to the LangChain, LangGraph, and Streamlit communities for their open tools and docs.


---

✅ Now you can:

- Paste this in `README.md` on GitHub or your local repo.
- Add a `requirements.txt` if needed.
- Commit with:

```bash
git add README.md
git commit -m "Added complete README for LangGraph project"
git push
