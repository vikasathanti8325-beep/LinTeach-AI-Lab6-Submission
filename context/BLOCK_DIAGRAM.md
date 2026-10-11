# LinTeach AI - System Block Diagram

## Overall System Architecture

```text
┌──────────────────────────────┐
│          STUDENT             │
│                              │
│  Enters Linear Algebra       │
│  question / attempt          │
└──────────────┬───────────────┘
               │
               │ Question
               ▼
┌──────────────────────────────┐
│       FRONTEND               │
│                              │
│ HTML + CSS + JavaScript      │
│                              │
│ • Input question             │
│ • Send request               │
│ • Display AI response        │
└──────────────┬───────────────┘
               │
               │ HTTP POST
               ▼
┌──────────────────────────────┐
│       FLASK BACKEND          │
│                              │
│ Python + Flask               │
│                              │
│ • Receive question           │
│ • Process request            │
│ • Load subject context       │
└──────────────┬───────────────┘
               │
               │ Context + Question
               ▼
┌──────────────────────────────┐
│    LINEAR ALGEBRA CONTEXT    │
│                              │
│ linear_algebra_context.md    │
│                              │
│ • Subject knowledge          │
│ • Teaching philosophy        │
│ • Difficulty levels          │
│ • Hint policy                │
│ • Teaching behavior          │
└──────────────┬───────────────┘
               │
               │ Teaching Instructions
               ▼
┌──────────────────────────────┐
│        OPENAI LLM            │
│                              │
│ Generates teaching response  │
│                              │
│ • Explanation                │
│ • Examples                   │
│ • Hints                      │
│ • Step-by-step solution      │
│ • Understanding checks       │
└──────────────┬───────────────┘
               │
               │ AI Response
               ▼
┌──────────────────────────────┐
│       FLASK BACKEND          │
│                              │
│ Returns response as JSON     │
└──────────────┬───────────────┘
               │
               │ HTTP Response
               ▼
┌──────────────────────────────┐
│          FRONTEND            │
│                              │
│ Displays teaching response   │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│          STUDENT             │
│                              │
│ Reads explanation, answers   │
│ follow-up questions, and     │
│ continues learning           │
└──────────────────────────────┘