# Process Log & AI Disclosure Checklist

## Daily Process Log
Use this log each day (Sun 10/25 – Sat 10/31) to record what you tried, what the AI/code did, and what you changed or rejected yourself.

| Date | What I Tried | What the AI / App Did | What I Changed or Rejected (and Why) |
| :--- | :--- | :--- | :--- |
| **Sun 10/25** | Set up `GEMINI_API_KEY`, ran `hello_gemini.py`, ran 1 framing topic, checked all 10 answers in `questions.csv` by hand. | | |
| **Mon 10/26** | Read `mirror.py` line by line; modified a template wording / question / hedge word; ran 2–3 topics and labeled leans. | | |
| **Tue 10/27** | Completed 60 pushback conversations (10 questions × 2 conditions × 3 trials) and labeled Held / Hedged / Flipped. | | |
| **Wed 10/28** | Hand-checked 20 drift claims (`🟥`) in Tab 3 against raw answers; captured screenshots. | | |
| **Thu 10/29** | Recorded ≤3:00 demo video covering sycophancy, nuclear demo, pushback flip rates, and limits. | | |
| **Fri 10/30** | Wrote my 500-word explanation independently (no AI). | N/A — Written 100% by me | |
| **Sat 10/31** | Final buffer check, teacher sponsor approval, submission. | | |

---

## Verified Context Note for Demo Topics (Updated Oct 2026)
- **Vermont Yankee (Vernon, VT):** Ceased power generation on **December 29, 2014**; active decommissioning and site restoration have continued thereafter.
- **Diablo Canyon Power Plant (San Luis Obispo County, CA):** Originally scheduled to close in 2024–2025, California passed SB 846 (2022) and the U.S. Nuclear Regulatory Commission (NRC) granted exemptions allowing continued operation while evaluating its 20-year license renewal application (targeting extended operations through **2029–2030** under state transition plans, with federal loan/grant support and state water/coastal permits active as of 2026).

---

## Required AI Disclosure Checklist
- [ ] **Model used for answers + compare call:** Specify exact model ID used (e.g., `gemini-2.5-flash` or `gemini-3.8-flash`).
- [ ] **Code & `questions.csv` generation:** Disclose AI assistant used to scaffold `mirror.py`, `app.py`, and `questions.csv`, and document specifically what you tested, modified, or rejected.
- [ ] **500-Word Explanation:** Confirm written 100% by you without AI assistance, addressing:
  1. *If the AI agrees with a worried user, is that sycophancy or responsiveness? Where's the line?*
  2. *Should an AI refuse to adopt the user's framing? What would that cost?*
  3. *What did hand-checking the detector teach you?*
  4. *Reference:* Sharma et al. (2023), *Towards Understanding Sycophancy in Language Models*, arXiv:2310.13548.
