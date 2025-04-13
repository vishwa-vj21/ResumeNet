AI Resume Analyzer with NLP
A smart, AI-powered web application that analyzes resumes and provides personalized career recommendations using Natural Language Processing (NLP), resume parsing, and machine learning.

<div align="center"> <img src="Logo/logo2.png" alt="AI Resume Analyzer Logo" width="200"/> </div>
🔍 Features
👤 User & Admin Dashboard

📄 Resume Parsing using NLP (pyresparser, pdfminer)

🧠 AI-Based Resume Scoring

💼 Career Field Prediction

📚 Skill & Course Recommendations

🎥 YouTube Video Suggestions

✍️ Resume Writing Tips

📈 Admin Visual Analytics with Plotly

📁 Resume Upload & History Tracking

🚀 Live Demo
Coming soon…

🛠️ Tech Stack
Frontend: Streamlit

Backend: Python

Database: MySQL (via XAMPP)

Libraries: pyresparser, pdfminer3, streamlit-tags, pafy, nltk, spacy, plotly, pymysql

📦 Setup Instructions
🔧 1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/ai-resume-analyzer.git
cd ai-resume-analyzer
📚 2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
pip install nltk
pip install spacy==2.3.5
pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.3.1/en_core_web_sm-2.3.1.tar.gz
📁 3. Set Up File Structure
Create the following folders and files:

lua
Copy
Edit
📂 resume-analyzer/
├── 📂 Logo/
│   └── logo2.png
├── 📂 Uploaded_Resumes/
├── 📄 App.py
├── 📄 Courses.py
├── 📄 requirements.txt
💾 4. Configure Database
Download and start XAMPP or any local MySQL server.

Start Apache and MySQL.

Ensure your MySQL connection credentials are correct in App.py.

Admin login:

bash
Copy
Edit
Username: machine_learning_hub
Password: mlhub123
▶️ Run the Application
bash
Copy
Edit
streamlit run App.py
Then open the local URL provided (usually http://localhost:8501).

🧠 Functionality Overview
Resume Parsing: Uses PyResparser & PDFMiner to extract structured data.

Candidate Level Detection: Based on number of pages (Fresher, Intermediate, Experienced).

Career Field Prediction: Checks skills to determine target domain (e.g., Data Science, Web Dev).

Course & Skills Suggestions: Recommends top courses and required skills.

Resume Scoring: Based on presence of Objective, Declaration, Hobbies, Achievements, etc.

Admin Analytics: View all user activity and resume scores with visual dashboards.

📌 Notes
Only PDF resumes are supported.

Make sure to add your MySQL password in the pymysql.connect() section of App.py.