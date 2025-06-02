# Professional-Persona-Agent - LLM-Powered Career Assistant for Real-Time Interaction

- ✨ **Transform your LinkedIn + Career Summary into a powerful, intelligent assistant.**

- 🤝 **Engage recruiters and hiring managers in real-time.**

- 🛠️ **Built using **Groq’s blazing-fast LLaMA 3.3 70B model**, Gradio, PDF parsing, and function-calling agents.**

- 🔔 **Pushover alerts + tool-based logic for user registration and unanswered question capture.**

---

## 🎯 Project Vision

Imagine having a version of *yourself*—trained on your **professional experience, achievements, and career goals**—interacting on your behalf, intelligently answering questions, and persuading recruiters or collaborators.

This project turns that vision into a **practical, deployable prototype**.

> 💡 **Use Case:** AI-powered digital persona that **represents your professional identity**—ideal for portfolio sites, networking, recruiting platforms, and career automation tools.

---

## 🚀 Demo Preview

🎥 Coming soon — but you can run it in 2 clicks via Colab.

[![Open In Colab](https://colab.research.google.com/drive/1-2I36TNX-rm85aMQx7_eCsHJUzVTlfoa?usp=sharing)

---

## 🧩 Features

| Feature | Description |
|--------|-------------|
| 💬 **LLM-Powered Chat** | Uses **LLaMA 3.3 70B** via Groq API for human-like, contextual responses |
| 📄 **LinkedIn & Summary Parsing** | Extracts content from your LinkedIn profile (PDF) and text summary |
| 🧠 **Professional Identity Emulation** | Chat agent fully adopts your name, tone, and expertise |
| 🔗 **Tool Calling (Function API)** | Registers: `Interested Users`, `Unanswered Questions` |
| 🔔 **Pushover Notifications** | Sends real-time updates when users register interest |
| 🧪 **Gradio UI** | Clean, interactive interface via Gradio’s chat interface |
| 📦 **Modular Structure** | Separated logic for tools, chat loops, environment variables |

---

## 🏢 Real-World & Industry Use Cases

> This project isn’t just a demo—it maps directly to real, high-value business applications.

### ✅ **For Job Seekers:**

- Host this on your portfolio site
  
- Let recruiters chat with your AI-powered professional persona
  
- Register interest directly with your email

### ✅ **For Recruiters:**

- Auto-screen candidates by chatting with their digital persona
  
- Identify strong profiles without scheduling initial calls

### ✅ **For Enterprises / Talent Platforms:**

- Deploy AI profiles for every team member
  
- Automate candidate evaluation
  
- Use as AI-enhanced employee bios for clients

---

## 🛠️ How It Works

### 📁 Data Flow:

1. Upload `LinkedIn PDF` + `Summary`
   
2. Extracts structured info using `PyPDF2` and text parsing
   
3. Injects into a **System Prompt** for LLaMA-3.3 (70B)
   
4. Chatbot interacts via Gradio with function-calling support
   
5. Calls `register_user_details()` or `register_unknown_question()` when needed
    
10. Sends real-time updates via `Pushover`

---

# Tech Stack

🧠 Groq API — Fast inference for LLaMA 3.3 70B

🤖 OpenAI (Optional) — Additional fallback if needed

📄 PyPDF2 — Extract text from LinkedIn PDF

💬 Gradio — Front-end chat interface

🔔 Pushover — Real-time push alerts

🛠️ Function Calling — Tool-use via structured JSON calls

---
# 📌 Sample Use Scenario

🧑 A recruiter visits your portfolio and chats with the AI persona:

Recruiter: What kind of backend frameworks have you worked with?

Agent: As Faiaz Ahmed, I've used Spring Boot extensively for microservices, REST APIs, and enterprise-grade applications...
Later...

Agent: I’d love to stay connected. Could you share your email so I can follow up?

🔔 You receive a Pushover alert:

“New interest registered: Recruiter from Acme Inc. with email john.doe@example.com”
