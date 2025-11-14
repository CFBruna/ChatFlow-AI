# 🤖 ChatFlow AI

[![Python](https://img.shields.io/badge/python-3.12-blue)](https://www.python.org/)
[![Django](https://img.shields.io/badge/django-5.2-green)](https://www.djangoproject.com/)
[![PostgreSQL](https://img.shields.io/badge/postgresql-16-blue)](https://www.postgresql.org/)
[![Docker](https://img.shields.io/badge/docker-ready-blue)](https://www.docker.com/)
[![LangChain](https://img.shields.io/badge/langchain-0.3-orange)](https://www.langchain.com/)
[![Groq](https://img.shields.io/badge/groq-llama--3.3--70b-purple)](https://groq.com/)

> AI-powered conversational assistant built with Django and LangChain  
![Demonstration](static/demo.git.gif)

📝 **Description**  

ChatFlow AI is a multi-user chatbot platform built with Django and powered by the Groq API (Llama 3.3 70B).  
Users can register, log in and chat with an AI assistant whose entire conversation history is saved.  
The system follows a production-ready structure using Docker, PostgreSQL, LangChain and environment-based configuration.

✨ **Features**  
- **User Authentication:** Full register/login with isolated user sessions  
- **Intelligent Chatbot:** Real-time responses via Groq API + LangChain  
- **Conversation Management:** Create, rename and delete with Ajax  
- **Conversation History:** Persistent chat history per user  
- **Responsive UI:** Clean layout with mobile-first design  
- **Production Ready:** Dockerized stack with health checks and optimized architecture  

🚀 **Tech Stack**  
- **Backend:** Python 3.12, Django 5.2, LangChain  
- **Database:** PostgreSQL 16  
- **API:** Groq (Llama 3.3 70B Versatile)  
- **Containerization:** Docker & Docker Compose  
- **Configuration:** Python Decouple (.env based)  

---

⚙️ **Getting Started**  
Run the project locally using Docker.

### Prerequisites  
- Docker  
- Docker Compose  
- Groq API Key (get yours at https://console.groq.com/)

---

### Step-by-step Guide

#### 1. Clone the repository:
```bash
git clone https://github.com/CFBruna/chatflow-ai.git
cd chatflow-ai
```

#### 2. Configure Your Environment:  
Copy `.env.example` and edit with your values (including `GROQ_API_KEY`):

```bash
cp .env.example .env
```

Inside `.env`, set:
```
GROQ_API_KEY=your_groq_api_key_here
SECRET_KEY=your-django-secret-key-here
```

#### 3. Build and Run the Application:
```bash
docker compose up --build
```

To run in background:
```bash
docker compose up -d --build
```

#### 4. Access the Application:
Open your browser:  
http://localhost:8000

The first build may take a few minutes.

---

### 🧑‍💻 Default Credentials  
A superuser is automatically created:

```
Username: admin
Password: admin123
```

⚠️ **Change these credentials immediately!**

---

🏗️ **Project Structure**
```
ChatFlow AI/
├── core/              # Django project settings
├── chatbot/           # Chat logic + LangChain integration
├── accounts/          # User authentication system
├── static/            # CSS, JS, images
├── staticfiles/       # Collected static files
├── Dockerfile         # Container definition
├── docker-compose.yml # Multi-container orchestration
├── entrypoint.sh      # Initialization script
└── requirements.txt   # Python dependencies
```

---

📜 **License**  
This project is licensed under the **MIT License**.  
➡️ Click here to view the license: **[LICENSE](LICENSE)**

---

👤 **Author**  
**Bruna Menezes**  
🔗 LinkedIn: https://www.linkedin.com/in/bruna-c-menezes/  
🐙 GitHub: https://github.com/CFBruna  
📧 Email: **brunaads.ti@gmail.com**

⭐ If this project helped you, consider leaving a star!
