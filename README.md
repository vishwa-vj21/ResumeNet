# 💼 AI Resume Analyzer with NLP

A smart, AI-powered web application that analyzes resumes and provides personalized career recommendations using Natural Language Processing (NLP), resume parsing, and machine learning.


---

## 🔍 Features

- 👤 **User & Admin Dashboard**
- 📄 **Resume Parsing** using NLP (`pyresparser`, `pdfminer`)
- 🧠 **AI-Based Resume Scoring**
- 💼 **Career Field Prediction**
- 📚 **Skill & Course Recommendations**
- 🎥 **YouTube Video Suggestions**
- ✍️ **Resume Writing Tips**
- 📈 **Admin Visual Analytics with Plotly**
- 📁 Resume Upload & History Tracking

---

## 🛠️ Tech Stack

- **Frontend:** Streamlit  
- **Backend:** Python  
- **Database:** MySQL (via XAMPP)  
- **Libraries:** `pyresparser`, `pdfminer3`, `streamlit-tags`, `pafy`, `nltk`, `spacy`, `plotly`, `pymysql`

---

## 📦 Setup Instructions

### 🔧 1. Clone the Repository

```bash
git clone https://github.com/yourusername/ai-resume-analyzer.git
cd ai-resume-analyzer
```

### 📚 2. Install Dependencies

Make sure you are using **Python 3.7 or 3.8** for compatibility.

```bash
pip install -r requirements.txt
pip install nltk
pip install spacy==2.3.5
pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.3.1/en_core_web_sm-2.3.1.tar.gz
```

### 🛠️ 3. Configure Database

1. **Download and start [XAMPP](https://www.apachefriends.org/index.html)** or any local MySQL server.
2. Start both **Apache** and **MySQL** from the control panel.
3. Ensure your MySQL connection credentials are correct in `App.py`:
   ```python
   mydb = mysql.connector.connect(
       host="localhost",
       user="your_username",
       password="your_password",
       database="your_database"
   )
   ```

### 🚀 4. Run the Application

Open your terminal and run:

```bash
streamlit run App.py
```