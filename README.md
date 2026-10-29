# 🎯 PrepPilot – AI-Powered Interview Trainer

An AI-powered interview preparation assistant built using **Langflow** and **IBM watsonx.ai** to help students practice interview questions, evaluate their answers, and improve their interview performance.

## 📌 Project Overview

PrepPilot is designed to make interview preparation more interactive and accessible. It uses a large language model to generate interview questions and provide feedback on student responses.

The project focuses on helping students prepare for technical and HR interviews through conversational AI.

## ✨ Key Features

* 🤖 **AI-Powered Interview Practice** — Practice interview questions using a conversational AI agent.
* 💻 **Multiple Interview Categories** — Designed to support HR, Python, SQL, Data Analysis, and Power BI.
* 📝 **Answer Evaluation** — Evaluate responses for correctness, relevance, clarity, and completeness.
* 📊 **Constructive Feedback** — Identify mistakes and areas that need improvement.
* 🚀 **Answer Improvement** — Generate improved, interview-ready answers.
* 🎯 **Personalized Practice Guidance** — Get suggestions for improving technical knowledge and communication skills.
* 📚 **Knowledge Base Integration** — Includes a Langflow Knowledge component configured with an interview knowledge base.

## 🛠️ Technology Stack

| Technology     | Purpose                                |
| -------------- | -------------------------------------- |
| Langflow       | Visual AI workflow development         |
| IBM watsonx.ai | Large language model integration       |
| IBM Granite    | AI model used for interview assistance |
| Python         | Supporting programming environment     |
| GitHub         | Project version control and sharing    |

## 🏗️ Project Architecture

The intended interview workflow is:

```text
                ┌─────────────────┐
                │   Chat Input    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Interview       │
                │ Trainer Agent   │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Answer          │
                │ Evaluation Agent│
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Interview Coach │
                │ Agent           │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │   Chat Output   │
                └─────────────────┘
```

**Note:** This diagram represents the intended multi-agent workflow. The individual agent components have been tested, but complete end-to-end evaluation and coaching behavior still require validation.

## ⚙️ Getting Started

### Prerequisites

Before using PrepPilot, make sure you have:

* Python installed.
* Langflow installed and running.
* An IBM Cloud account.
* Access to IBM watsonx.ai and a compatible language model.
* An IBM watsonx.ai project with the required machine learning service associated.

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/shubhamofficial1508-debug/PrepPilot-Interview-Trainer.git
```

**2. Navigate to the project directory**

```bash
cd PrepPilot-Interview-Trainer
```

**3. Install Langflow**

If Langflow is not already installed, create a Python virtual environment and install it:

```bash
python -m venv venv
```

Activate the environment on Windows:

```bash
venv\Scripts\activate
```

Install Langflow:

```bash
pip install langflow
```

**4. Start Langflow**

```bash
langflow run
```

Open the local URL displayed in the terminal, typically:

`http://localhost:7860`

**5. Import the workflow**

* Open Langflow.
* Import the exported PrepPilot JSON workflow.
* Configure the IBM watsonx.ai credentials and project settings.
* Verify that the selected model is available.
* Run the workflow and test its responses.

**Important:** The exported JSON file contains the workflow configuration. It does not automatically provide IBM Cloud credentials, guarantee model access, or install every required dependency.

## 🧪 Example Use Cases

### 1. Interview Practice

**Input:**

```text
Start a mock interview for a Data Analyst internship.
Ask one question at a time.
```

**Expected behavior:** The interview agent asks a relevant question and waits for the student's answer.

### 2. Answer Evaluation

**Input:**

```text
Evaluate my answer.

Question: What is Python?

My answer: Python is a programming language used for data analysis and automation.
```

**Expected behavior:** The evaluation agent assesses the answer, explains any missing details, and suggests an improved response.

### 3. Interview Coaching

**Input:**

```text
Help me improve my technical interview answers.
```

**Expected behavior:** The coaching agent provides practical preparation suggestions based on the answer and evaluation feedback supplied.

*These examples describe intended behavior. Actual outputs depend on the configured model, instructions, and workflow connections.*

## 🔐 Security

* Never publish API keys, access tokens, passwords, or other confidential credentials.
* Do not export sensitive credentials with the workflow.
* Store secrets securely and configure credentials locally.
* Review exported JSON files before uploading them to GitHub.

## 🚧 Current Development Status

* [x] Initial Langflow workflow created.
* [x] IBM watsonx.ai model configured and tested.
* [x] Interview Trainer Agent created and tested individually.
* [x] Answer Evaluation Agent created and tested individually.
* [x] Interview Coach Agent created and tested individually.
* [x] Workflow exported as a JSON file.
* [ ] Validate the complete multi-agent workflow from input to output.
* [ ] Verify that the knowledge base retrieves relevant interview material.
* [ ] Test answer evaluation against correct and incorrect responses.
* [ ] Improve error handling and response consistency.
* [ ] Add workflow screenshots and a project demonstration.

## 🎯 Future Enhancements

* Retrieval-Augmented Generation (RAG) for knowledge-grounded answers.
* More accurate answer scoring and structured feedback.
* Difficulty-based interview question selection.
* Interview performance tracking.
* Support for additional technical subjects.
* A user-friendly web interface.
* Interview history and progress reports.

## 👨‍💻 Author

**Shubham**

B.Tech Computer Science & Engineering
Interested in Data Analytics, Artificial Intelligence, and AI-powered applications.

GitHub: [@shubhamofficial1508-debug](https://github.com/shubhamofficial1508-debug)

## 📄 License

This project is currently available for learning and demonstration purposes. A formal open-source license can be added to the repository if needed.

---

⭐ **If you find PrepPilot interesting, consider starring the repository!**

*Built as a learning project exploring conversational AI, visual workflow development, and interview preparation.*
