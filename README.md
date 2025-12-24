# PDF AI Summarizer

A simple web application to summarize PDF documents using Google Gemini API.
Users can upload a PDF file and receive an AI-generated summary through a clean web interface.

## Tech Stack

### Frontend / UI:

    - Next.js (React-based web framework)
    - Tailwind CSS (optional styling)

### Backend / Processing:

    - Python 3.10+
    - Flask (API server)
    - PyPDF2 (PDF text extraction)
    - Google Gemini API (LLM summarization)
    - python-dotenv (environment variable management)

## Features

    - Upload PDF files for summarization
    - Extract text from PDF documents
    - Generate AI summaries using Google Gemini (gemini-2.5-flash)
    - Language selection for summaries (EN / ID)
    - Clean and minimal UI
    - Backend API for PDF processing and AI interaction
    - Easily extendable architecture

## Requirements

    - Python 3.10 or higher
    - Node.js 18+
    - pip (Python package manager)
    - Google Gemini API key
    - Windows / Linux / macOS

## Installation

1. Clone the repository

   git clone <repo-url>
   cd pdf-ai-sum

2. Install dependencies

### Backend:
    - cd be
    - pip install -r requirements.txt

### Frontend:
    - cd fe
    - npm install

3. Setup API Key

   Create a .env file inside the Backend folder:

   GEMINI_API_KEY=your_google_gemini_api_key_here

## Running the App

### Backend:
    - cd be
    - python main.py

Backend will run on: http://127.0.0.1:8000

### Frontend:
    - cd fe
    - npm run dev

Frontend will run on: http://localhost:3000

## Usage

    - Open the web interface in your browser
    - Upload a PDF file
    - Select the summary language (optional)
    - Click Generate Summary
    - Read, copy, or save the generated summary