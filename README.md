# AI Productivity Assistant

**CAPACITI AI Skill Accelerator Programme — Project Submission**

A Python CLI AI assistant built with **Gemini 3.5 Flash** that automates five
common workplace tasks, demonstrates structured prompt engineering, and applies
responsible AI practices.

---

## Problem Statement

Professionals spend significant time on repetitive tasks: drafting emails,
summarising meetings, planning schedules, and researching topics. This project
delivers an AI-driven assistant that automates those processes, improving
productivity and decision-making.

---

## Features

| # | Feature | Description |
|---|---------|-------------|
| 1 | **Smart Email Generator** | Drafts professional emails with tone (formal / informal / persuasive) and audience (client / manager / team) adaptation |
| 2 | **Meeting Notes Summarizer** | Converts raw notes into a structured report: summary, key points, decisions, action items, next steps |
| 3 | **AI Task Planner / Scheduler** | Prioritises tasks with the Eisenhower Matrix and builds a time-blocked daily or weekly plan |
| 4 | **AI Research Assistant** | Summarises articles/reports and produces insights, recommendations, and limitations |
| 5 | **Interactive AI Chatbot** | Multi-turn workplace assistant with optional token-by-token streaming |

---

## Tools Used

| Tool | Purpose |
|------|---------|
| Python 3.10+ | Core language |
| **Gemini 3.5 Flash** (`gemini-3.5-flash`) | Large language model for all AI features |
| `google-genai` | Official Google Gen AI Python SDK |
| `python-dotenv` | Environment variable management |
| `argparse`, `logging`, `re` | CLI, audit logging, and pattern matching |

**Model specs (Gemini 3.5 Flash):**
- Model ID: `gemini-3.5-flash` (stable, generally available)
- Context window: 1,048,576 tokens
- Max output: 65,536 tokens
- Modalities: text, audio, image, video, code

---

## Installation

### Prerequisites
- Python 3.10+
- A Gemini API key: https://aistudio.google.com/apikey

### Steps

```bash
# 1. Create project folder
mkdir ai-productivity-assistant && cd ai-productivity-assistant
# Save the four files: app.py, requirements.txt, .gitignore, README.md

# 2. Create virtual environment
python -m venv venv

# macOS / Linux
source venv/bin/activate

# Windows PowerShell
.\venv\Scripts\Activate.ps1

# 3. Install dependencies
pip install -r requirements.txt

# 4. Add your API key
echo "GEMINI_API_KEY=your_api_key_here" > .env
