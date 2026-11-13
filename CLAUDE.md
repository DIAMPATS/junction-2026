# Junction 2026 Project Rules

## Sponsor APIs & Environment Variables
- Primary Inference: Verda Nemotron 3.5 Super VL (`VERDA_INFERENCE_KEY`)
- Multimodal / Secondary: Google Gemini (`GEMINI_API_KEY`)
- Live Web Search / Scraping: Exa (`EXA_API_KEY`) & Context.dev (`CONTEXT_DEV_API_KEY`)
- Cloud GPUs: Modal (`MODAL_TOKEN_ID`, `MODAL_TOKEN_SECRET`)

## Folder Ownership (Avoid Merge Conflicts)
- `firmware/` -> Embedded / Arduino UNO Q / Wendy edge code
- `backend/` -> Python FastAPI + AI inference pipelines
- `frontend/` -> Web UI / dashboard

## Rules
- Never hardcode API keys; always load from `.env`.
- Keep functions modular and include a quick CLI test command for new modules.
- Do not put Obsidian or coding agents inside Docker.
