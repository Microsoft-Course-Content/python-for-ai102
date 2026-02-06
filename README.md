# 🐍 python-for-ai102

> **Learn only the Python you need for Microsoft AI-102 labs — 6 Jupyter Notebooks covering foundations to Azure SDK patterns. Free & open-source.**

[![GitHub](https://img.shields.io/badge/License-MIT-blue.svg)](#-license)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python&logoColor=white)](#-software-requirements)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange?logo=jupyter)](#-repository-contents)
[![AI-102](https://img.shields.io/badge/Microsoft-AI--102-purple?logo=microsoft)](#-ai-102-lab-repositories-for-after-this-course)

---

## 📌 Purpose

Microsoft's [AI-102: Designing and Implementing a Microsoft Azure AI Solution](https://learn.microsoft.com/en-us/training/courses/ai-102t00) labs are now **Python-only**. Students who are new to Python often struggle to follow the lab code — not because of the AI concepts, but because they can't read the Python.

This course bridges that gap. It teaches **only the Python you need** to confidently read, understand, and modify code in AI-102 lab exercises. No fluff — every example connects directly to patterns found in the official Microsoft Learning GitHub repositories.

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   Student with         This Course          Ready for           │
│   no Python    ───────────────────────►    AI-102 Labs          │
│   experience          (6 hours)                                 │
│                                                                 │
│                  ┌─────────────────────┐                        │
│                  │  Python Basics      │                        │
│                  │  Data Structures    │                        │
│                  │  Functions & Modules│                        │
│                  │  Files & Config     │                        │
│                  │  REST APIs          │                        │
│                  │  Azure AI Patterns  │                        │
│                  └─────────────────────┘                        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 🎯 Who Is This For?

| Audience | Benefit |
|----------|---------|
| 🎓 Students new to Python | Learn Python through AI-102 relevant examples |
| 🧑‍🏫 MCT / Trainers | Ready-made 6-hour pre-course module |
| 💼 IT Pros switching to AI | Quick ramp-up before certification prep |
| 🔄 C# developers | Understand Python equivalents for AI-102 labs |

---

## 📂 Repository Contents

```
python-for-ai102/
│
├── 📓 01_Python_Foundations.ipynb           ← Notebook 1
├── 📓 02_Data_Structures.ipynb             ← Notebook 2
├── 📓 03_Functions_Modules_ErrorHandling.ipynb  ← Notebook 3
├── 📓 04_Files_JSON_DotEnv.ipynb           ← Notebook 4
├── 📓 05_REST_APIs.ipynb                   ← Notebook 5
├── 📓 06_Complete_AI102_Pattern.ipynb      ← Notebook 6
│
├── 📄 requirements.txt       ← All Python packages needed
├── 🔐 .env.example           ← Sample environment variables template
└── 📄 README.md              ← You are here
```

---

## 🗺️ Course Outline — Notebook Details

### 📓 Notebook 1: Python Foundations (~1 hour)

> *"Before you can talk to Azure AI, you need to speak Python."*

| Topic | AI-102 Relevance |
|-------|-------------------|
| `print()` function | Display API responses, debug output |
| Variables & assignment | Store endpoints, API keys, results |
| Data types (`str`, `int`, `float`, `bool`) | Understand what kind of data you're working with |
| String operations | URL building, text manipulation |
| **f-strings** (formatted strings) | Used in every single AI-102 lab |
| `input()` | Interactive labs that take user text |
| Basic arithmetic | Confidence scores, percentages |
| Comments | Reading lab code annotations |

---

### 📓 Notebook 2: Data Structures (~1 hour)

> *"Azure AI responses are lists of dictionaries. Master these two, and you can parse anything."*

| Topic | AI-102 Relevance |
|-------|-------------------|
| Lists `[]` | Collections of entities, phrases, objects |
| Indexing & slicing | Access specific results |
| `for` loops | Process each item in a response |
| `enumerate()` | Loop with position tracking |
| Dictionaries `{}` | **JSON responses map directly to dicts** |
| `.get()` safe access | Avoid crashes on missing keys |
| **Nested structures** | Navigate real API response trees |
| List comprehensions | Filter results concisely |

---

### 📓 Notebook 3: Functions, Modules & Error Handling (~1 hour)

> *"AI-102 labs organize code into functions — and always wrap API calls in try/except."*

| Topic | AI-102 Relevance |
|-------|-------------------|
| Defining functions (`def`) | Every lab has functions like `analyze_text()` |
| Parameters & return values | Pass text in, get results back |
| Default parameters | Optional settings like `language="en"` |
| `if/elif/else` | Handle different sentiments, check thresholds |
| `while` loops | Continuous input loops in labs |
| `import` statements | Load Azure SDKs and utilities |
| `os` module | **Environment variables, file paths** |
| `json` module | **Parse API responses** |
| `try/except/finally` | **Graceful error handling** |

---

### 📓 Notebook 4: Files, JSON & .env Configuration (~1 hour)

> *"Every AI-102 lab starts by loading a .env file. Every response is JSON. Every Vision lab reads an image file."*

| Topic | AI-102 Relevance |
|-------|-------------------|
| Reading text files | Analyze reviews, documents |
| Writing files | Save results |
| `.env` file pattern | **Store API keys securely** |
| `load_dotenv()` + `os.getenv()` | **The first 3 lines of every lab** |
| `json.load()` / `json.dump()` | Read/write JSON config & results |
| `json.loads()` / `json.dumps()` | Parse API response strings |
| Binary file reading (`"rb"`) | **Send images to Vision API** |
| `os.listdir()` + `os.path.join()` | Batch-process files in a folder |

---

### 📓 Notebook 5: REST APIs & HTTP Requests (~1 hour)

> *"At the heart of every Azure AI service is a REST API. Learn the request-response cycle."*

| Topic | AI-102 Relevance |
|-------|-------------------|
| HTTP methods (GET, POST) | POST data for analysis, GET results |
| Request anatomy (URL, headers, body) | Build complete API requests |
| `Ocp-Apim-Subscription-Key` header | **Azure API authentication** |
| `Content-Type` headers | JSON vs binary (images) |
| `response.status_code` | Check for success or errors |
| `response.json()` | Parse the result |
| HTTP status codes | Debug 401, 403, 429 errors |
| Query parameters | API version, feature selection |
| Sending binary image data | Vision API pattern |

---

### 📓 Notebook 6: The Complete AI-102 Pattern (~1 hour)

> *"All 5 notebooks come together. This is what real AI-102 lab code looks like."*

| Topic | AI-102 Relevance |
|-------|-------------------|
| **REST API client pattern** | Language Detection lab structure |
| **SDK client pattern** | Text Analytics with `TextAnalyticsClient` |
| **Computer Vision pattern** | Image analysis with caption, tags, objects |
| **Batch file processing** | Analyze all files in a folder |
| Quick reference cheat sheet | Copy-paste patterns for labs |
| `pip install` reference table | Every Azure SDK package you'll need |

---

## 💻 System Requirements

### Hardware

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| RAM | 4 GB | 8 GB |
| Disk Space | 2 GB free | 5 GB free |
| Internet | Required for AI-102 labs | Required for AI-102 labs |

> **Note:** The 6 training notebooks themselves work **offline** — no Azure subscription or internet needed. Internet and Azure credentials are only needed when you move to actual AI-102 lab exercises.

### Operating System

| OS | Supported |
|----|-----------|
| Windows 10/11 | ✅ Yes |
| macOS 12+ | ✅ Yes |
| Ubuntu 20.04+ / Linux | ✅ Yes |

---

## 🛠️ Software Requirements

### Required Software

| Software | Version | Purpose | Download |
|----------|---------|---------|----------|
| **Python** | 3.9 or higher | Run all notebooks and labs | [python.org/downloads](https://www.python.org/downloads/) |
| **Jupyter Notebook** or **JupyterLab** | Latest | Run `.ipynb` files interactively | Installed via `pip` (see below) |
| **VS Code** *(recommended)* | Latest | Code editor with Jupyter support | [code.visualstudio.com](https://code.visualstudio.com/) |

### VS Code Extensions (Recommended)

| Extension | Publisher | Purpose |
|-----------|-----------|---------|
| Python | Microsoft | Python language support |
| Jupyter | Microsoft | Run notebooks inside VS Code |
| Pylance | Microsoft | IntelliSense for Python |

### For AI-102 Labs (After This Course)

| Software | Purpose |
|----------|---------|
| Azure CLI | Manage Azure resources from terminal |
| Git | Clone Microsoft Learning lab repos |
| Azure Subscription | Deploy and use AI services |

---

## 🚀 Setup & Installation

### Step 1 — Install Python

Download and install Python 3.9+ from [python.org](https://www.python.org/downloads/).

> ⚠️ **Windows users:** Check the box **"Add Python to PATH"** during installation.

Verify installation:

```bash
python --version
```

### Step 2 — Clone or Download This Repository

```bash
# Option A: Using Git
git clone https://github.com/<your-org>/python-for-ai102.git
cd python-for-ai102

# Option B: Download ZIP and extract from GitHub
# Then navigate to the extracted folder
```

### Step 3 — Create a Virtual Environment (Recommended)

```bash
# Create virtual environment
python -m venv venv

# Activate it
# Windows:
venv\Scripts\activate

# macOS / Linux:
source venv/bin/activate
```

### Step 4 — Install Dependencies

```bash
pip install -r requirements.txt
```

> 💡 **Tip:** For the 6 training notebooks only, you just need the Section 1 packages. The full `requirements.txt` also includes Azure SDKs for when you move to actual labs.

### Step 5 — Set Up Environment Variables (For AI-102 Labs)

```bash
# Copy the example file
cp .env.example .env

# Edit .env with your actual Azure credentials
# Replace placeholder values with your keys and endpoints
```

### Step 6 — Launch Jupyter Notebook

```bash
# Option A: Classic Jupyter
jupyter notebook

# Option B: JupyterLab
jupyter lab

# Option C: VS Code
# Just open the .ipynb file — VS Code handles the rest
```

### Step 7 — Start Learning!

Open `01_Python_Foundations.ipynb` and begin. 🎉

---

## 📋 How to Use This as a Trainer

### Suggested 6-Hour Schedule

| Time | Notebook | Trainer Notes |
|------|----------|---------------|
| **Hour 1** (0:00–1:00) | 01 — Python Foundations | Start slow. Let students type along. Explain f-strings thoroughly — they'll see them everywhere. |
| **Hour 2** (1:00–2:00) | 02 — Data Structures | Focus heavily on **dictionaries** and **nested structures**. This is the #1 skill for parsing API responses. |
| **Hour 3** (2:00–3:00) | 03 — Functions & Modules | Emphasize `os`, `json`, and `try/except`. Walk through the AI-102 error handling pattern. |
| *Break* (3:00–3:15) | ☕ 15-minute break | |
| **Hour 4** (3:15–4:15) | 04 — Files, JSON & .env | Do the `.env` section live — show how `load_dotenv()` works. This demystifies the first 5 lines of every lab. |
| **Hour 5** (4:15–5:15) | 05 — REST APIs | Draw the request/response diagram on a whiteboard. Explain headers, status codes. |
| **Hour 6** (5:15–6:15) | 06 — Complete AI-102 Pattern | This is the payoff. Walk through each pattern and show the equivalent code from an actual AI-102 lab repo. |

### Trainer Tips

- **Run every code cell live** — don't just show slides
- **Encourage students to modify code** — change variables, break things, see what happens
- **Connect to AI-102 constantly** — after each concept, say *"In the AI-102 lab, you'll see this when..."*
- **Use the practice exercises** — give students 3–5 minutes to try on their own
- **Notebook 6 is the bridge** — after this, open an actual AI-102 lab and show students they can now read the code

---

## 🔗 AI-102 Lab Repositories (For After This Course)

Once students complete these 6 notebooks, they're ready for the official labs:

| Repository | Covers |
|------------|--------|
| [mslearn-ai-services](https://github.com/MicrosoftLearning/mslearn-ai-services) | Azure AI Services (provisioning, security, monitoring) |
| [mslearn-ai-vision](https://github.com/MicrosoftLearning/mslearn-ai-vision) | Computer Vision, Image Analysis, OCR |
| [mslearn-ai-language](https://github.com/MicrosoftLearning/mslearn-ai-language) | Text Analytics, NLP, Language Understanding |
| [mslearn-ai-document-intelligence](https://github.com/MicrosoftLearning/mslearn-ai-document-intelligence) | Form Recognizer, Document Intelligence |
| [mslearn-knowledge-mining](https://github.com/MicrosoftLearning/mslearn-knowledge-mining) | Azure AI Search, Knowledge Mining |
| [mslearn-openai](https://github.com/MicrosoftLearning/mslearn-openai) | Azure OpenAI, Generative AI |

> 📖 **Official Course Page:** [AI-102T00: Designing and Implementing a Microsoft Azure AI Solution](https://learn.microsoft.com/en-us/training/courses/ai-102t00)

---

## 📖 Python Concepts ↔ AI-102 Labs Quick Map

For quick reference — which Python concept maps to which AI-102 lab activity:

```
Python Concept              Where You'll See It in AI-102
─────────────────────       ─────────────────────────────────
f-strings                   Building API URLs, printing results
dictionaries                EVERY API response is a dictionary
nested dict/list            Parsing sentiment scores, entities
json.loads()                Parsing REST API response body
os.getenv()                 Loading endpoint & key from .env
try/except                  Wrapping every API call
requests.post()             Calling REST APIs directly
with open("img","rb")       Sending images to Vision API
for item in list            Processing each detected entity
client.method()             Using Azure SDK clients
pip install                 Installing Azure SDK packages
```

---

## ❓ Troubleshooting

| Problem | Solution |
|---------|----------|
| `python` command not found | Use `python3` instead, or reinstall Python and check "Add to PATH" |
| `pip` command not found | Use `python -m pip install` instead |
| Jupyter won't start | Run `pip install jupyter notebook` then try again |
| `ModuleNotFoundError` | Run `pip install -r requirements.txt` |
| Notebooks won't open in VS Code | Install the "Jupyter" extension from Microsoft |
| `.env` values not loading | Make sure file is named `.env` (not `.env.example`) and is in the same folder |
| Azure API returns 401 | Double-check your API key in the `.env` file |
| Azure API returns 403 | Check your resource's region and endpoint URL |

---

## 🏷️ GitHub Topics

Add these topics to your repo for discoverability:

```
python  ai-102  azure  microsoft-certification  jupyter-notebook
azure-ai  mct  python-tutorial  azure-ai-services  cloud-computing
```

---

## ⭐ Support This Project

If this helped you or your students:

- ⭐ **Star** the repo — it helps others find it
- 🍴 **Fork** it — customize for your classroom
- 📢 **Share** it — tag someone prepping for AI-102

---

## 📜 License

This material is created for educational purposes. Feel free to use, modify, and distribute for training and learning.

---

## 🙏 Acknowledgments

- [Microsoft Learning AI-102 Lab Repositories](https://github.com/MicrosoftLearning) — for the lab code patterns these notebooks are based on
- [Microsoft Learn — AI-102 Course](https://learn.microsoft.com/en-us/training/courses/ai-102t00) — official course curriculum
- [AI-102 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-102) — exam skills measured

---

> *Built with ❤️ to help every student succeed in AI-102.*
