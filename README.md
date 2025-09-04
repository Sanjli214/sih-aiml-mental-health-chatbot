# sih-aiml-mental-health-chatbot
🤖 AI/ML module for Smart India Hackathon project — a digital mental health support chatbot for students

This repository contains the **AI/ML contribution** for the Smart India Hackathon (SIH) Problem Statement:  

**"Development of a Digital Mental Health and Psychological Support System for Students in Higher Education"**.

---

## 📂 Project Structure
SIH_AIML_Module/
├── data/ # Student-focused dataset (JSON + CSV)
├── scripts/ # Training + API + augmentation
├── notebooks/ # (Optional) Colab-ready notebook
├── requirements.txt # Dependencies
├── README.md # Documentation

---

## ⚡ Features
- **Custom Dataset (200+ Q&A pairs)** for students:
  - Exam Stress, Sleep Issues, Loneliness, Peer Pressure, Career Anxiety, Burnout, Crisis
- **Fine-Tuning BlenderBot** on student-specific conversations
- **Paraphrasing Script** to augment dataset automatically
- **Flask API** for chatbot deployment
- **Crisis Detection** (keywords + referral)
- **Streamlit UI** (to be integrated by frontend team)
- **MySQL Logging** for chat + screening data

---

## 🚀 Quickstart

### 1. Install dependencies
pip install -r requirements.txt
2. Train the Model
bash
Copy code
python scripts/train_blenderbot.py --data_path data/student_mental_health_dataset.json
3. Run Flask API
bash
Copy code
python scripts/inference_api.py
4. Paraphrase & Augment Dataset
bash
Copy code
python scripts/paraphrase.py --input data/student_mental_health_dataset.csv --output data/augmented_dataset.csv
🧩 Tech Stack
Python (3.9+)

Hugging Face Transformers

BlenderBot (facebook/blenderbot-400M-distill)

Flask + Streamlit

MySQL (storage + analytics)

📊 Dataset
JSON: data/student_mental_health_dataset.json

CSV: data/student_mental_health_dataset.csv

Covers multiple student issues with empathetic responses

👨‍💻 Contributors
AIML Module: Chatbot, Dataset, Fine-tuning

Backend/Frontend: Teammates (Flask, Streamlit, DB integration)

⚠️ Safety Note
This chatbot is not a replacement for professional help.
In case of severe distress, students should be referred to counsellors or helplines.

---


Ask ChatGPT
