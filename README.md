# KnowItAll – PDF Chatbot (RAG)

Upload PDFs and ask questions. Answers are grounded in your documents, with page references.

## How it works (RAG pipeline)
1. **Ingest** – PDF.js extracts text page by page.
2. **Chunk** – text is split into 120-word overlapping passages.
3. **Retrieve** – BM25 ranking finds the top 4 passages for the question.
4. **Generate** – Gemini writes an answer using only those passages (optional API key). Without a key, the best matching sentences are shown.

## Run locally
Open `index.html` in a browser. No install or backend needed.

## Deploy
Drag this folder onto https://app.netlify.com/drop, or import the GitHub repo in Vercel.

## Tech
HTML, CSS, JavaScript, PDF.js, BM25, Google Gemini API
