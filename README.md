# 🩸 Blood Work Analyzer

An AI-powered blood report analysis tool that extracts abnormal values, generates a plain-language health summary, and recommends a personalized Indian diet plan — powered by Google Gemma (gemma-4-31b-it) via LangChain.

### Project Structure

blood-work-analyzer/

│

├── app.py                      # Streamlit web application (main UI)

├── Blood_Work_Analysis.ipynb   # Jupyter Notebook

├── blood_work.txt              # Sample blood report

├── .env                        # API key storage

├── requirements.txt            # Python dependencies

└── README.md                   # Project documentation

### 🧠 What It Does
This project takes a raw blood work report as text input and runs it through a two-stage LLM pipeline:
StageWhat HappensStage 1 – ExtractionParses all test values and classifies each as HIGH, LOW, or NORMAL based on the report's reference rangesStage 2 – InterpretationGenerates a 4–5 line plain-English health summary + a practical Indian diet plan (foods to eat / foods to avoid)

### 🖥️ Application Overview
app.py — Streamlit Web App
A clean, two-column web interface:

Left panel — Paste your blood work report and click Analyze
Right panel — Displays scrollable output boxes for:

🫀 Health Summary
🥗 Suggested Indian Diet Plan
