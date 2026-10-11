# LinTeach AI - Project Plan

## 1. Project Title

**LinTeach AI - AI Teaching Agent for Linear Algebra**

---

## 2. Project Objective

The objective of this project is to develop an interactive AI Teaching Agent that helps students learn Linear Algebra through personalized, step-by-step guidance.

Instead of simply providing answers, the system is designed to explain concepts, provide examples, give hints, identify mistakes, and check the student's understanding.

---

## 3. Problem Statement

Students often struggle to understand mathematical concepts because traditional question-answer systems may provide only a final answer.

LinTeach AI addresses this problem by acting as a teaching assistant that guides students through the learning process.

---

## 4. Target Users

The primary users are:

- Undergraduate students
- Engineering students
- Students learning Linear Algebra
- Beginners who need intuitive explanations
- Students who need guided problem-solving support

---

## 5. Subject Scope

The teaching agent focuses on Linear Algebra topics including:

- Vectors
- Matrices
- Systems of Linear Equations
- Gaussian Elimination
- Rank
- Null Space
- Determinants
- Matrix Inverse
- Eigenvalues
- Eigenvectors
- Diagonalization
- Linear Transformations
- Inner Products
- Orthogonality
- Gram-Schmidt Process
- Least Squares

---

## 6. System Components

### Frontend

The frontend provides an interactive interface where students can enter their questions and view the teaching agent's responses.

Technology:

- HTML
- CSS
- JavaScript

### Backend

The backend receives student questions, loads the subject-specific context, communicates with the LLM, and returns the generated teaching response.

Technology:

- Python
- Flask
- Flask-CORS

### LLM

An OpenAI Large Language Model is used to generate the teaching responses.

### Subject Context

A Markdown file contains Linear Algebra knowledge and detailed instructions defining how the AI should behave as a teaching agent.

File:

```text
context/linear_algebra_context.md