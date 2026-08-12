# 🤖 AI Interview Question Designer

An AI-powered **Interview Question Designer** that generates professional interview questions and detailed answers based on a candidate's **job role** and **experience level**.

Built with **Python, Streamlit, OpenRouter, and OpenAI-compatible APIs**, this application helps students, job seekers, and developers prepare for technical interviews efficiently.

---

## 🚀 Features

* 🤖 AI-generated interview questions
* 💼 Job-role based questions
* 📈 Experience-level customization
* 📝 Detailed answers for every question
* 💡 Interview evaluation tips
* 💻 Coding questions
* 🧠 Concept-based questions
* 🎯 Scenario-based questions
* 🔧 Problem-solving questions
* 🏗️ System-design questions
* 📂 Project-based questions
* 🔍 Technical deep-dive questions
* 📥 Download generated questions and answers
* 🎨 Modern and responsive Streamlit interface
* 🖥️ Command-line version also included

---

## 🧠 How It Works

The application takes two inputs:

1. **Job Role**
2. **Experience Level**

The AI then generates a customized interview preparation document.

```text
             Job Role
                │
                ▼
        Experience Level
                │
                ▼
          InterviewTask
                │
                ▼
        AI Prompt Generation
                │
                ▼
           OpenRouter AI
                │
                ▼
     Interview Questions
                │
                ▼
       Detailed Answers
                │
                ▼
      Interview Evaluation
                │
                ▼
        Download Report
```

---

## 📚 Question Categories

The AI generates questions across multiple categories:

| Category               | Description                             |
| ---------------------- | --------------------------------------- |
| 🧠 Concept             | Tests fundamental technical knowledge   |
| 🎯 Scenario            | Tests real-world decision making        |
| 🧩 Problem Solving     | Tests analytical and logical thinking   |
| 💻 Coding              | Tests programming ability               |
| 🔬 Technical Deep Dive | Tests advanced technical knowledge      |
| 📂 Project             | Tests practical project experience      |
| 🏗️ System Design      | Tests architecture and design knowledge |

---

## 📊 Experience Levels

The Streamlit application supports:

```text
Fresher
1 Year
2 Years
3 Years
5 Years
8+ Years
```

The generated questions are adjusted according to the selected experience level.

---

## 🖥️ Application Interface

The application provides a simple interface containing:

### Job Role

Enter a role such as:

```text
Python Developer
AI Engineer
Data Scientist
Machine Learning Engineer
Full Stack Developer
Data Analyst
```

### Experience Level

Select the candidate's experience.

### Generate

Click:

```text
🚀 Generate Interview Questions & Answers
```

The AI then prepares the interview questions and answers.

---

## 📄 Generated Output

Each question follows a structured format:

```text
================================================

📌 Question 1

Category:
Concept

Question:
What is Python?

✅ Answer:
Detailed professional explanation...

⭐ Interview Evaluation:
What a strong candidate should mention...

================================================
```

The generated answers may include:

* Definition
* Explanation
* Working
* Practical examples
* Interview evaluation points

---

## 🛠️ Technologies Used

### Frontend

* Streamlit
* HTML
* CSS

### Backend

* Python

### AI

* OpenRouter API
* OpenAI Python SDK
* `openai/gpt-4o-mini`

### Configuration

* python-dotenv

---

## 📁 Project Structure

```text
AI Interview Questions/
│
├── app.py
├── agent.py
├── task.py
├── main.py
├── requirements.txt
├── .gitignore
│
└── 03_interview_questions/
    ├── agent.py
    ├── main.py
    ├── task.py
    └── requirements.txt
```

---

## 📄 File Description

### `app.py`

The main Streamlit application.

It handles:

* Job role input
* Experience selection
* AI generation
* Result display
* Error handling
* Downloading interview questions

---

### `task.py`

Contains the `InterviewTask` class.

It:

* Creates the AI prompt
* Sends the request to OpenRouter
* Configures the AI model
* Generates interview questions and answers
* Returns the generated content

---

### `agent.py`

Contains the `InterviewQuestionAgent` class.

It provides another AI-based interface for generating interview questions according to:

* Job role
* Experience level

---

### `main.py`

Provides a command-line version of the application.

Run it from the terminal to generate interview questions without Streamlit.

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
```

Navigate into the project:

```bash
cd "AI Interview Questions"
```

---

### 2. Create a Virtual Environment

Windows:

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

macOS/Linux:

```bash
source venv/bin/activate
```

---

### 3. Install Dependencies

Make sure your `requirements.txt` contains:

```text
openai
python-dotenv
streamlit
```

Then install:

```bash
pip install -r requirements.txt
```

---

## 🔑 API Configuration

Create a `.env` file in the project directory:

```env
OPENROUTER_API_KEY=your_openrouter_api_key
```

The application uses the OpenRouter API endpoint:

```text
https://openrouter.ai/api/v1
```

The configured AI model is:

```text
openai/gpt-4o-mini
```

### ⚠️ Important

Never upload your API key to GitHub.

Your `.gitignore` should contain:

```text
.env
.env.txt
venv/
.venv/
__pycache__/
*.pyc
```

If an API key has already been exposed publicly, **revoke it and create a new key**.

---

## ▶️ Run the Streamlit Application

Start the application with:

```bash
streamlit run app.py
```

The application will normally be available at:

```text
http://localhost:8501
```

---

## 🖥️ Run the CLI Version

You can also run the command-line version:

```bash
python main.py
```

The application will ask:

```text
💼 Enter Job Role:
📈 Enter Experience Level:
```

It will then generate the interview questions and answers in the terminal.

---

## 💡 Example

### Input

```text
Job Role:
Python Developer

Experience:
Fresher
```

### Output

The AI generates questions covering areas such as:

```text
1. Python Fundamentals
2. Object-Oriented Programming
3. Data Structures
4. Exception Handling
5. File Handling
6. SQL
7. Problem Solving
8. Coding
9. Projects
10. Technical Scenarios
11. System Design
```

Each question includes a detailed answer and interview evaluation guidance.

---

## 📥 Download Feature

After generating the interview preparation document, users can click:

```text
📥 Download Questions & Answers
```

The application downloads the generated content as:

```text
AI_Interview_Questions_Answers.txt
```

---

## 🎯 Who Can Use This?

This project is useful for:

* 🎓 Students
* 👨‍💻 Freshers
* 💼 Job seekers
* 🧑‍💼 Working professionals
* 🧠 Developers
* 🤖 AI/ML candidates
* 📊 Data Science candidates
* 🔍 Interview preparation

---

## 🌟 Benefits

### For Freshers

Get beginner-friendly questions based on the selected job role.

### For Experienced Candidates

Prepare for deeper technical, scenario-based, project, and system-design questions.

### For Developers

Practice coding and technical questions before an interview.

### For Students

Use AI-generated questions for interview preparation and technical learning.

---

## 🔮 Future Improvements

Possible future enhancements:

* 📄 Resume upload
* 🎯 Resume-based interview questions
* 💼 Job Description-based questions
* 🧠 Personalized interview preparation
* 🎤 AI mock interview
* 🗣️ Voice-based interview
* ⭐ Interview performance scoring
* 📊 Candidate performance dashboard
* ⏱️ Timed interview mode
* 💬 Follow-up questions
* 📑 PDF report generation
* 📚 Question history
* 🌐 Multi-language support

---

## 🔐 Security Best Practices

Never commit these files or folders:

```text
.env
.env.txt
venv/
.venv/
__pycache__/
```

Never hard-code API keys inside Python files.

Use environment variables instead:

```python
import os
from dotenv import load_dotenv

load_dotenv()

api_key = os.getenv("OPENROUTER_API_KEY")
```

---

## 🤝 Contributing

Contributions are welcome!

### 1. Fork the repository

### 2. Create a new branch

```bash
git checkout -b feature/new-feature
```

### 3. Make your changes

### 4. Commit your changes

```bash
git add .
git commit -m "Add new interview feature"
```

### 5. Push your branch

```bash
git push origin feature/new-feature
```

### 6. Create a Pull Request

---

## 📜 License

This project is intended for **educational and personal use**.

You are free to modify and extend the project for your own learning and development.

---

## 👨‍💻 Author

**Arun Naik**

Built with ❤️ using:

```text
Python
Streamlit
OpenRouter AI
OpenAI SDK
HTML
CSS
```

---

## ⭐ Support

If you find this project useful, please consider giving the GitHub repository a ⭐.

It helps support the project and encourages further development.
