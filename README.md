# 📄 PDF Summarizer

A fullstack web application that lets you upload PDF documents and get AI-powered summaries instantly. Built with a **Python** backend and a **TypeScript** frontend.

---

## ✨ Features

- Upload PDF files and extract text automatically
- Generate concise AI-powered summaries
- Clean and responsive web interface
- RESTful API backend

---

## 🗂️ Project Structure

```
pdf-summarizer/
├── be/          # Backend — Python (FastAPI / Flask)
└── fe/          # Frontend — TypeScript (React / Next.js)
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.9+
- Node.js 18+
- npm or yarn

---

### ⚙️ Backend Setup

```bash
cd be

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows

# Install dependencies
pip install -r requirements.txt

# Copy and configure environment variables
cp .env.example .env
# Edit .env and add your API key(s)

# Run the server
uvicorn main:app --reload       # or: python app.py
```

The backend will be available at `http://localhost:8000`.

---

### 🖥️ Frontend Setup

```bash
cd fe

# Install dependencies
npm install

# Copy and configure environment variables
cp .env.example .env.local
# Edit .env.local — set NEXT_PUBLIC_API_URL=http://localhost:8000 (or equivalent)

# Run the development server
npm run dev
```

The frontend will be available at `http://localhost:3000`.

---

## 🔑 Environment Variables

### Backend (`be/.env`)

| Variable      | Description              | Required |
|---------------|--------------------------|----------|
| `API_KEY`     | AI provider API key      | ✅ Yes   |

### Frontend (`fe/.env.local`)

| Variable              | Description           | Required |
|-----------------------|-----------------------|----------|
| `NEXT_PUBLIC_API_URL` | Backend API base URL  | ✅ Yes   |

---

## 🛠️ Tech Stack

| Layer    | Technology               |
|----------|--------------------------|
| Frontend | TypeScript, React/Next.js, CSS |
| Backend  | Python, FastAPI/Flask    |
| AI       | LLM / Summarization API  |

---

## 🤝 Contributing

1. Fork this repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📝 License

This project is open source. See [LICENSE](LICENSE) for details.
