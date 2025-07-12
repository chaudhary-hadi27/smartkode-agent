# 🚀 SmartKode WhatsApp AI Chatbot

Welcome to the **SmartKode Institute's AI WhatsApp Chatbot** — a complete, production-grade assistant powered by FastAPI, Twilio, and Groq's LLaMA3. This chatbot engages students via WhatsApp, guiding them on SmartKode's AI, Web Development, and Data courses.

---

## 📦 Features

* 🤖 AI Assistant powered by **Groq’s LLaMA3-8B**
* 💬 WhatsApp Integration using **Twilio API**
* 🧠 Per-user temporary memory for personalized chat flow
* 🔕 **Ignore list** support for private numbers (e.g. family)
* 💾 Saves all chats to JSON in `chat_logs/`
* 📊 Visual chat dashboard with editable names using **Streamlit**
* 🔄 Session auto-resets after inactivity (10 min timeout)
* 🔐 Secure `.env` for API keys and tokens

---

## 🗂️ Project Structure

```
SK-Learning-Bot/
├── app/
│   ├── config.py           # Loads environment variables
│   ├── dashboard.py        # Streamlit GUI with chat logs & user mapping
│   ├── handlers.py         # Main chat handler logic
│   ├── groq_api.py         # (Optional) Groq response helper
├── main.py                 # FastAPI webhook for Twilio
├── chat_logs/              # Per-user conversation histories
├── requirements.txt        # All dependencies
├── .env                    # API credentials (not committed)
```

---

## ⚙️ Requirements

### 🔐 Environment Variables (`.env`)

```env
GROQ_API_KEY=your_groq_key_here
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_ACCOUNT_SID=your_twilio_account_sid
```

> ⚠️ Do **not** share or commit your `.env` file publicly.

---

## 🚀 Getting Started (Local)

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/SK-Learning-Bot.git
cd SK-Learning-Bot
```

### 2. Create & Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # (Linux/macOS)
venv\Scripts\activate     # (Windows)
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Backend (FastAPI)

```bash
uvicorn main:app --host 0.0.0.0 --port 8000
```

### 5. Run Dashboard (Streamlit GUI)

```bash
streamlit run app/dashboard.py
```

---

## 📚 SmartKode Courses (Included in Prompt)

### 💡 AI Courses

* Machine Learning
* Deep Learning
* Natural Language Processing
* Computer Vision
* Generative AI
* AI Chatbots

### 🌐 Web Development

* HTML, CSS, JavaScript
* React.js, Next.js
* API Integration
* Task Automation

### 📊 Data Skills

* Excel
* SQL
* Data Analysis
* Dashboards & Visualization

---

## 🧠 Bot Commands

| Command | Description                 |
| ------- | --------------------------- |
| `reset` | Clears current user session |


---

## 🙌 Contributing

Pull requests are welcome. Let's make this the most student-friendly AI bot ever.

---

## 👨‍💻 Created by [SmartKode Institute](https://smartkode.io)

Empowering students with cutting-edge skills in AI, Web, and Data. 🚀
# smartkode-agent
