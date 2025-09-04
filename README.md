🎓 SIH AIML Module - Digital Mental Health Chatbot

🤖 This repository contains the AI/ML module for the Smart India Hackathon (SIH) Problem Statement:
"Development of a Digital Mental Health and Psychological Support System for Students in Higher Education"

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![HuggingFace](https://img.shields.io/badge/Transformers-HuggingFace-yellow.svg)
![Flask](https://img.shields.io/badge/Backend-Flask-lightgrey.svg)
![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-red.svg)
![MySQL](https://img.shields.io/badge/Database-MySQL-orange.svg)
![Status](https://img.shields.io/badge/Project-SIH%202025-brightgreen.svg)

📌 About

College students often face stress, anxiety, depression, and burnout.
This chatbot provides a confidential, stigma-free digital support system with empathetic AI-driven responses and early screening.

This repo focuses on the AIML component:

Training and fine-tuning a student-focused chatbot

Augmenting dataset for better performance

Providing a Flask API for backend integration

Supporting a Streamlit frontend for deployment

📂 Project Structure

sih-aiml-mental-health-chatbot/
│
├── data/                                   # Datasets for training & evaluation
│   ├── student_mental_health_dataset.json  # Main dataset (JSON format)
│   ├── student_mental_health_dataset.csv   # Main dataset (CSV format)
│   └── augmented_dataset.csv               # (Optional) Generated via paraphrasing
│
├── scripts/                                # Your chatbot scripts
│   ├── train_blenderbot.py                 # Fine-tuning BlenderBot on student dataset
│   ├── inference_api.py                    # Flask API to serve chatbot
│   └── paraphrase.py                       # Augment dataset with paraphrasing
│
├── requirements.txt                        # Python dependencies
└── README.md                               # Documentation (your explanation of AIML work)


⚡ Features

Student-specific dataset (200+ Q&A pairs)
Covers: exam stress, sleep issues, loneliness, peer comparison, career anxiety, burnout, crisis support

Fine-tuned BlenderBot (facebook/blenderbot-400M-distill)

Empathetic emotional responses (not rule-based if-else only)

Crisis detection with emergency referral

Flask API for backend integration

Streamlit UI (handled by frontend team)

MySQL storage for chat + screening logs

🚀 Quickstart
1. Clone repo
git clone https://github.com/your-username/sih-aiml-mental-health-chatbot.git
cd sih-aiml-mental-health-chatbot

2. Install dependencies
pip install -r requirements.txt

3. Train the Model
python scripts/train_blenderbot.py --data_path data/student_mental_health_dataset.json

4. Run Flask API
python scripts/inference_api.py

5. Augment Dataset
python scripts/paraphrase.py --input data/student_mental_health_dataset.csv --output data/augmented_dataset.csv

🧩 Tech Stack

Python 3.9+

Hugging Face Transformers

BlenderBot (facebook/blenderbot-400M-distill)

Flask (backend API)

Streamlit (frontend UI)

MySQL (logging + analytics)

📊 Dataset

student_mental_health_dataset.json → JSON format

student_mental_health_dataset.csv → CSV format

Categories:

Exam Stress

Sleep Issues

Loneliness

Peer Comparison

Career Anxiety

Burnout

Crisis situations

👨‍💻 Contributors

AIML Module: Sanjli Agarwal (Chatbot, dataset, fine-tuning, API)

Backend/Frontend: Teammates (Flask, Streamlit, MySQL integration)

⚠️ Safety Disclaimer

This chatbot is designed as a supportive companion, not a replacement for professional medical advice.
If a student shows severe distress, the system redirects to helplines/counsellors.
