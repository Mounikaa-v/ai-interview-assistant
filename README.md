# AI Interview Assistant — Merged Mode

This project unifies **Resume-Aware OpenAI Mode** (if `VITE_OPENAI_API_KEY` exists) and a **Randomized Mock Mode** fallback (2 Easy, 2 Medium, 2 Hard from a larger pool). It includes:

- Resume upload + parsing (PDF/DOCX/TXT best-effort client-side)
- Resume-aware AI question generation (OpenAI) or randomized mock fallback
- Interviewer Dashboard with **search, sort, score badges, and summaries**
- Candidate detail page with **chat history (Q/A), profile, and AI summary**
- Local persistence via **localStorage** and a **Welcome Back** modal on Home
- Tailwind polished UI

## Quick Start

```bash
npm i
npm run dev
```

Optionally create `.env` at root:

```
VITE_OPENAI_API_KEY=sk-...
```

Build & preview:

```bash
npm run build
npm run preview
```

## Notes

- PDF/DOCX parsing is best-effort on the client. For high-fidelity text, integrate a server parser.
- Scoring is a placeholder (length-based). Replace with rubric + AI evaluation if desired.
