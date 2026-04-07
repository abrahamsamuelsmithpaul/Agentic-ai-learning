```markdown
# 🚀 AI Career Conversation Assistant — Let’s Learning with Sam

An AI-powered conversational assistant that represents my professional profile and interacts like a virtual version of me. This project enables real-time conversations, answers questions about my experience, and intelligently captures potential leads.

🔗 **Live App:**  
https://huggingface.co/spaces/AbrahamSamuel/career_conversation

---

## 📌 Overview

This application uses Large Language Models (LLMs) to simulate a professional conversation interface. It can:

- Answer questions about my skills and experience  
- Maintain contextual conversations  
- Detect user intent and contact information  
- Trigger real-time notifications for potential opportunities  

---

## ✨ Features

### 🤖 Conversational AI
- Built with **Gradio** for interactive UI  
- Powered by **OpenAI GPT models**  
- Maintains chat history for context-aware responses  

---

### 📄 Personalized Knowledge Base
- Extracts data from:
  - LinkedIn PDF  
  - Custom summary file  
- Dynamically injects context into responses  

---

### 🎯 Intelligent Lead Detection
- Detects:
  - Email addresses  
  - Phone numbers  
  - Intent keywords (e.g., *“contact me”, “let’s connect”*)  
- Avoids unnecessary triggers — only captures meaningful leads  

---

### 🔔 Real-Time Notifications
- Integrated with **Pushover API**  
- Sends alerts when:
  - User shares contact info  
  - Shows hiring/connection intent  

---

### ☁️ Cloud Deployment
- Deployed on **Hugging Face Spaces**  
- Uses **Secrets** for secure API key management  
- Works both locally and in production  

---

## 🛠️ Tech Stack

- **Language:** Python  
- **AI/LLM:** OpenAI (GPT-4o-mini)  
- **Frontend:** Gradio  
- **Backend:** Python  
- **Notifications:** Pushover API  
- **Deployment:** Hugging Face Spaces  
- **Data Sources:** PDF + Text  

---

## 🏗️ Architecture

```

User → Gradio UI → Chat Function
↓
OpenAI API (LLM Response)
↓
Lead Detection (Regex + Keywords)
↓
Pushover API (Notification)

```

---

## 📂 Project Structure

```

labs/
├── app.py
├── requirements.txt
├── me/
│    ├── linkedin.pdf
│    └── summary.txt

````

---

## ⚙️ Setup Instructions

### 1. Clone Repo
```bash
git clone https://github.com/your-username/your-repo.git
cd labs
````

---

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3. Create `.env` (for local)

```
OPENAI_API_KEY=your_key
PUSHOVER_TOKEN=your_token
PUSHOVER_USER=your_user
```

---

### 4. Run Locally

```bash
python app.py
```

---

## 🔐 Hugging Face Deployment

Add these in **Settings → Secrets**:

```
OPENAI_API_KEY=sk-xxxx
PUSHOVER_TOKEN=xxxx
PUSHOVER_USER=xxxx
```

Then deploy:

```bash
uv run gradio deploy
```

---

## 🧪 Example Usage

### ❌ No Notification

* "Hi"
* "Tell me about your skills"

### ✅ Notification Triggered

* "My email is [abc@gmail.com](mailto:abc@gmail.com)"
* "Call me at 9876543210"
* "Let’s connect"
* "I’m interested in hiring"

---

## 🚧 Challenges Solved

* Managing environment variables across local & cloud
* Debugging OpenAI + Pushover integrations
* Handling Gradio message formats
* Avoiding noisy notifications with smart filtering
* Fixing deployment/runtime issues

---

## 🚀 Future Enhancements

* Store leads in database (PostgreSQL / SQLite)
* Add RAG (Retrieval-Augmented Generation)
* Build analytics dashboard
* Add authentication
* Integrate LangChain / LlamaIndex

---

## 💼 Resume Highlight

**Built and deployed an AI-powered conversational assistant with intelligent lead detection and real-time notification system using OpenAI, Gradio, and Hugging Face Spaces.**

---

## 📢 Let’s Learning with Sam

Sharing practical AI and data engineering learnings through hands-on projects.

---

## ⭐ Feedback

Feel free to try the app and share your feedback!


