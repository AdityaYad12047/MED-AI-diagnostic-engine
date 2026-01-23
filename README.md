
                                                                                ```
                                                                                ███╗   ███╗   ███████╗  █████╗      █████╗   ██╗
                                                                                ████╗ ████║   ██╔════╝  ██╔══██╗   ██╔══██╗  ██║
                                                                                ██╔████╔██║   █████╗    ██   ██║   ███████║  ██║
                                                                                ██║╚██╔╝██║   ██╔══╝    ██╔══██╗   ██╔══██║  ██║
                                                                                ██║ ╚═╝ ██║   ███████╗  █████║     ██║  ██║  ██╗
                                                                                ╚═╝     ╚═╝   ╚══════╝  ╚═╝ ╚═╝    ╚═╝  ╚═╝  ╚═╝
                                                                                     MULTI-MODAL DIAGNOSTIC ENGINE
                                                                                ```

---
# 🚑 MedAI — Multi-Modal Diagnostic Engine & ICU Risk Prediction System  
AI-driven medical analysis using **vitals, imaging, and multimodal models** (XGBoost + Google Gemini 2.5 Flash).

<p align="center">
  <img src="https://github.com/AdityaYad12047/MED-AI-diagnostic-engine/blob/main/static/Gemini_Generated_Image_3bnino3bnino3bni.png" />
</p>

---

## 🔥 Overview  
MedAI is an advanced **clinical decision-support prototype** that analyzes:

- ICU bedside vitals  
- X-rays, MRIs, ECG strips  
- Blood reports & PDFs  
- Clinical notes & structured text  

It combines a **rule-based ICU scoring model**, an **XGBoost deterioration risk predictor**, and **Gemini multimodal AI** to generate:

- ICU admission probability  
- Color-coded risk index  
- Explainable clinical findings  
- Multimodal medical summaries  
- PDF + Image analysis JSON  

This system is designed for **educational, research, and demonstrative purposes**.

---

## 🧠 Tech Stack

### **Backend**
- Python  
- Flask  
- XGBoost  
- Google Gemini 2.5 Flash API  
- NumPy, Pandas

### **Frontend**
- HTML5 / CSS3  
- Chart.js (Donut risk graph)  
- Responsive UI with animations

### **Modeling**
- Rule-Based ICU Deterioration Score  
- XGBoost Calibration Model  
- Gemini Multimodal Model for imaging, ECGs, PDFs

---

## 📊 Features

### **1. ICU Vitals Risk Engine**
- Inputs: **Age, HR, BP, RR, Temperature, SpO₂, WBC**
- Hybrid model:
  - Rule-based ICU thresholds  
  - XGBoost model trained on **39,000+ labelled clinical datapoints**
- Output:
  - **0–100% calibrated ICU risk score**  
  - ICU admission probability  
  - Explainable, human-readable findings  

### **2. Multimodal Medical Analysis (Gemini 2.5 Flash)**
- Upload:
  - X-ray  
  - MRI  
  - ECG strip  
  - Lab report PDF  
  - Clinical notes  
- Returns:
  - Risk severity (Low → Critical)  
  - Extracted abnormalities  
  - Structured JSON for dashboards  
  - Condensed medical summarization  

### **3. Clean UI + Animations**
- Fade-in diagnostic cards  
- Donut-style risk visual  
- Loading overlay with progress bar  
- Fully responsive layout  

---

## 🏗 Project Structure

```
MED-AI-diagnostic-engine/
│
├── models/
│   └── vitals_xgb.pkl
│
├── static/
│   └── style.css
│
├── templates/
│   └── index.html
│
├── uploads/
│
├── app.py
├── model_engine.py
├── LICENSE
├── README.md
└── .gitignore
```

---

## 🚀 How to Run Locally

### **1. Clone the repository**
```bash
git clone https://github.com/AdityaYad12047/MED-AI-diagnostic-engine.git
cd MED-AI-diagnostic-engine
```

### **2. Create virtual environment**
```bash
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate   # Mac/Linux
```

### **3. Install dependencies**
```bash
pip install -r requirements.txt
```

### **4. Add your Gemini API Key**
Create a `.env` file:
```
GEMINI_API_KEY=your_api_key_here
```

### **5. Run the app**
```bash
python app.py
```

Open browser →  
**http://127.0.0.1:5000**

---

## 🌍 Deployment Guide

### **Deploy on Render (Recommended)**
1. Push repo to GitHub.
2. Go to: https://render.com  
3. Create **New Web Service**
4. Select your repo  
5. Set:
   ```
   Build Command: pip install -r requirements.txt
   Start Command: gunicorn app:app
   ```
6. Add environment variable:
   ```
   GEMINI_API_KEY=xxxx
   ```
7. Deploy.

---

### **Deploy on Railway**
1. Go to: https://railway.app  
2. Create a new project → Deploy from GitHub  
3. Add environment variables  
4. Railway auto-detects Flask  
5. Deploy.

---

## 🎥 Demo Video Script (2–3 Minutes)

### **Introduction**
“Hello, today I will present **MedAI** – a multi-modal diagnostic engine designed for ICU risk prediction and medical image interpretation.”

---

### **Slide: System Overview**
“This system combines vital-sign analysis, imaging analysis, and rule-based ICU scoring with an XGBoost machine learning model trained on over **39,000 clinical datapoints**.”

---

### **Slide: Architecture**
“The system has two major engines:

1. **ICU Vitals Risk Engine**  
   - Uses vitals such as HR, BP, SpO₂, RR, Temp, WBC.  
   - A hybrid model computes a calibrated 0–100% risk score.

2. **Multimodal AI Engine**  
   - Powered by Gemini 2.5 Flash.  
   - Interprets X-rays, MRIs, ECGs, PDFs and returns structured clinical findings.”

---

### **Slide: UI & Workflows**
“The frontend includes animated cards, a donut-style risk indicator, and a smooth loading overlay.  
The backend is built using Flask, Python, and Chart.js.”

---

### **Slide: Real-time Demo**
“In the web app, users upload vitals or imaging, and the model instantly produces:

- ICU admission probability  
- Risk band (Low, Moderate, High, Critical)  
- Clinical findings  
- Multimodal interpretation outputs.”

---

### **Closing**
“This system demonstrates how modern AI models can combine structured and unstructured medical data to support ICU triage and diagnostic workflows.  
Thank you.”

---

# 🎨 GitHub Banner (ASCII)

```
███╗   ███╗   ███████╗  █████╗      █████╗   ██╗
████╗ ████║   ██╔════╝  ██╔══██╗   ██╔══██╗  ██║
██╔████╔██║   █████╗    ██   ██║   ███████║  ██║
██║╚██╔╝██║   ██╔══╝    ██╔══██╗   ██╔══██║  ██║
██║ ╚═╝ ██║   ███████╗  █████║     ██║  ██║  ██╗
╚═╝     ╚═╝   ╚══════╝  ╚═╝ ╚═╝    ╚═╝  ╚═╝  ╚═╝
     MULTI-MODAL DIAGNOSTIC ENGINE
```

---


