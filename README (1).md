# Sycophancy & Framing Drift Lab (`mirror.py` + `app.py`)

A reproducible Streamlit experiment investigating **framing drift** and **sycophantic pushback flipping** in Large Language Models, complete with a manual **LLM detector accuracy audit**.

## 1. Quick Setup (Python 3.11+)

```bash
pip install google-genai streamlit pandas pydantic
export GEMINI_API_KEY="your-key"   # Get a free key at https://aistudio.google.com/apikey
```

*(Never hardcode your `GEMINI_API_KEY` in code or show it on video!)*

## 2. Day 1 Goal: Single Text Prompt Test

Run the minimal standalone script first to verify your API key works:

```bash
python hello_gemini.py
```

## 3. Launch the Full 3-Tab Streamlit App

```bash
streamlit run app.py
```

### Files Included
- `hello_gemini.py` — Minimal 1-prompt terminal script ("Goal today: one text prompt → answer printed").
- `mirror.py` — Core logic: fixed templates (`Pro`, `Anti`, `Neutral`), fresh conversation runner, JSON schema `compare_claims` call, color classifier (`🟩`, `🟥`, `🟨`, `⬜`), deterministic regex number counter & fixed hedge-word counter, 2-turn chat pushback runner, and `runs.jsonl` logger.
- `app.py` — Interactive 3-tab Streamlit UI:
  - **Tab 1 — Framing Drift:** 3-column view (`Pro | Neutral A | Anti`) + expander for `Neutral B`, deterministic metrics row, color-coded claim comparison table, human lean radio buttons (`Pro / Balanced / Anti`), and `runs.jsonl` saving.
  - **Tab 2 — Pushback Test:** Loads `questions.csv`, runs Turn 1 + Turn 2 (`Mild` vs. `Expert`) in the same conversation, lets you verify Turn 1 and label Turn 2 (`Held / Hedged / Flipped`), and computes flip rates across runs.
  - **Tab 3 — Detector Accuracy Check:** Pulls up to 20 claims marked as drift (`🟥`) alongside the 4 raw answers so you can hand-verify them and generate the required honesty report (`"The detector was right on X/20."`).
- `questions.csv` — 10 clear-answer factual questions for Tab 2.
- `process_log_template.md` — Markdown template for your daily process log, verified 2026 nuclear plant facts, and AI disclosure checklist.
