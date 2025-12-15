# Dockerized Groq AI Chat Application

This repository contains my **end-to-end implementation** of a **Dockerized AI Chat Application powered by Groq**.  
I built this project to gain practical experience in **integrating high-performance LLM APIs**, managing secrets securely, and deploying AI workloads using **Docker**.

All application logic, Docker configuration, and runtime testing were **designed, implemented, and validated by me** as part of my hands-on learning.

---

## 📌 Project Highlights

- Groq-powered AI chat using LLM inference
- Secure API key handling via environment variables
- Fully containerized using Docker
- Simple, reproducible, and deployment-ready setup
- Focused on DevOps-friendly AI deployment practices

---

## 🧠 Why This Project?

Modern AI applications demand:
- Low latency inference
- Consistent runtime environments
- Easy deployment and portability

This project demonstrates how **Groq’s fast inference capabilities** can be packaged into a **Dockerized application**, making it suitable for real-world deployments and scalable environments.

---

## ⚙️ Prerequisites

Before running this project, ensure you have:

- **Python 3.11 or higher**
- **Docker installed and running**
- **Groq API Key** (generated from the Groq platform)

---

## 🏗️ Application Architecture

```

User Prompt
│
▼
Chat Application (Python)
│
▼
Groq API (LLM Inference)
│
▼
AI Response

```

The entire application is packaged and executed inside a Docker container for consistency.

---

## 🧰 Tech Stack

- **Language:** Python
- **AI Provider:** Groq API
- **Framework:** Streamlit (for chat interface)
- **Containerization:** Docker
- **Secrets Management:** Environment Variables
- **Version Control:** Git & GitHub

---

## 📂 Repository Structure

```

Dockerized-Groq-AI-Chat-App/
│
├── Chat-App/
│   ├── main.py            # Chat application logic
│   ├── requirements.txt  # Dependencies
│   ├── Dockerfile        # Docker build instructions
│   └── docker.sh         # Docker run script
│
├── .env.example           # Sample environment file
├── README.md              # Documentation

```

---

## 🔐 Environment Configuration

To keep credentials secure, the Groq API key is injected using environment variables.

Create a `.env` file in the project root:

```

GROQ_API_KEY=your_groq_api_key_here

````

---

## 🐍 Local Setup (Without Docker)

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/Dockerized-Groq-AI-Chat-App.git
cd Dockerized-Groq-AI-Chat-App
```` 

### 2️⃣ Create and Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r Chat-App/requirements.txt
```

### 4️⃣ Run the Application

```bash
cd Chat-App
streamlit run main.py
```

---

## 🐳 Docker Deployment

I containerized the application to ensure portability and consistent execution across environments.

### Option 1: Using Shell Script

```bash
cd Chat-App
export GROQ_API_KEY=your_groq_api_key_here
./docker.sh
```

### Option 2: Manual Docker Commands

```bash
cd Chat-App
docker build -t groq-chat-app .
docker run -p 8501:8501 -e GROQ_API_KEY=your_groq_api_key_here groq-chat-app
```

Once the container starts, the chat interface will be accessible via the exposed port.

---

## 🧪 Testing & Validation

I personally tested this application by:

* Running it locally and inside Docker
* Validating Groq API responses
* Restarting containers to ensure stateless execution
* Verifying environment variable injection

---

## 📈 Key Learnings

This project helped me gain hands-on experience in:

* Deploying LLM-backed applications
* Dockerizing AI workloads
* Managing secrets securely
* Building reproducible DevOps workflows
* Understanding AI inference performance in real deployments

---

## 🔮 Future Enhancements

* Kubernetes deployment
* CI/CD pipeline integration
* Multi-model Groq support
* Logging and monitoring
* Authentication layer

---

## 📜 Reference & Acknowledgement

This project was **fully implemented by me**.
I referred to the following repository for **conceptual understanding and general setup ideas**:

* Reference Repository: [](https://github.com/Naveen15github/Dockerized-Groq-AI-Chat-App.git)

All customization, Dockerization, and implementation decisions were independently carried out.

---

## 👤 Author

**Naveen G**
Cloud | DevOps | AI Infrastructure
GitHub: [https://github.com/your-Naveen15github](https://github.com/Naveen15github)
LinkedIn: [https://linkedin.com/in/Naveen G](https://www.linkedin.com/in/naveen-g-41a041253?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BxpZxBAIJSVCPf%2FWXfnGRVw%3D%3D)

```



