# Gemini API Integration – Hacktiv8 Project

This project is created as part of a **Hacktiv8 project task**, demonstrating the integration of Google's **Gemini API** using Node.js and Express. The application allows users to generate AI responses based on different types of input:

- Text
- Image
- Document
- Audio

---

## Features

Generate AI content from:
- Plain text prompts  
- Uploaded images  
- Uploaded documents (PDF, DOCX, etc.)  
- Audio files (MP3, WAV, etc.)

Uses [Google GenAI SDK](https://www.npmjs.com/package/@google/genai) and the `gemini-2.5-flash` model.

RESTful API endpoints for easy integration.

---

## Prerequisites

- Node.js (v18 or newer)
- Google Gemini API Key  

---

API Endpoints
- POST /generate-text

Generate response from a text prompt.
Body (JSON):
{
  "prompt": "Explain..."
}

- POST /generate-from-image

Generate response using a text prompt and an uploaded image.
Form Data:
image: The image file (e.g., PNG, JPG)
prompt: Text prompt

- POST /generate-from-document

Generate response using a document and optional prompt.
Form Data:
document: PDF or DOCX file
prompt: Text prompt

- POST /generate-from-document

Generate response using a document and optional prompt.
Form Data:
document: PDF or DOCX file

- POST /generate-from-audio

Generate transcript or response from an audio file.
Form Data:
audio: MP3 or WAV file
