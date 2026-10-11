# LinTeach AI

## AI Teaching Agent for Linear Algebra

LinTeach AI is an interactive AI-based teaching agent designed to help students learn Linear Algebra through step-by-step explanations, examples, hints, and understanding checks.

The system adapts its explanations according to the student's level and focuses on helping the student understand the concept rather than simply providing the final answer.

---

## Features

- Interactive student interface
- Natural-language question answering
- Linear Algebra focused teaching
- Step-by-step explanations
- Beginner, Intermediate, and Advanced level support
- Hints before revealing answers
- Worked examples
- Follow-up questions
- Understanding checks
- Correction of incorrect attempts
- Subject-specific knowledge context
- LLM-powered responses
- Secure API key management using `.env`

---

## Technologies Used

- Python
- Flask
- Flask-CORS
- OpenAI API
- HTML
- CSS
- JavaScript
- Markdown
- Python Virtual Environment

---

## Project Structure

```text
LinTeach-AI/
│
├── backend/
│   ├── __init__.py
│   └── app.py
│
├── context/
│   └── linear_algebra_context.md
│
├── frontend/
│   └── frontend/
│       └── index.html
│
├── .env
├── .gitignore
├── README.md
└── venv/