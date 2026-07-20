# doctronic-safe-ai-starter

Fork, clone, and harden a vulnerable AI prescription system inspired by the real Doctronic incident: build safe validation, audit trails, and tests from scratch.

## The Incident

In January 2026, an AI system called Doctronic accepted a fabricated regulatory bulletin and generated a dangerously incorrect prescription dosage recommendation. 
No input validation. No audit trail. No safety checks. Full writeup: [`docs/incident-summary.md`](docs/incident-summary.md). Over the course of today, you'll rebuild it into something safer, one module at a time.

## What You'll Build

Work through these in order. Check off each one as you commit your fix — your commit history becomes the story of how you hardened this system.

- [ ] **APIs & REST (FastAPI)** — Understand how the vulnerable endpoint currently works
- [ ] **Variables & Data Types (Pydantic)** — Add schema validation to the bulletin input
- [ ] **Logic & Conditions** — Add dosage-safety checks and guardrails
- [ ] **Loops & Automation** — Automate repeated validation/checks across inputs
- [ ] **Functions & OOP (Agent Patterns)** — Refactor into agent-style structure
- [ ] **Databases & Audit Trails** — Log every decision so failures are traceable
- [ ] **Testing & Governance** — Add automated tests to catch regressions
- [ ] **Data Visualization Fundamentals** — Learn chart grammar, chart selection, and how to spot misleading charts
- [ ] **Streamlit** — Build an interactive dashboard to surface the system's audit trail and safety checks

## Getting Started

1. **Fork this repo** (top right → Fork) — this creates your own copy under your GitHub account
2. **Clone your fork** (not this original!):
   ```bash
   git clone https://github.com/<your-username>/doctronic-safe-ai-starter.git
   cd doctronic-safe-ai-starter
   ```
3. **Set up your environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate      # Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
4. **Commit as you go**, at each checkpoint above:
   ```bash
   git add .
   git commit -m "Add Pydantic validation to bulletin input"
   git push origin main
   ```

## Repo Structure

```
doctronic-safe-ai-starter/
|── README.md #the overview - this document
├── docs/
│   └── incident-summary.md   # the real case, in brief
├── app/
│   ├── main.py                # FastAPI entrypoint
│   ├── models/                 # you'll add Pydantic schemas here
│   ├── routes/
│   │   └── bulletin.py         # the vulnerable endpoint — fix this
│   ├── db/                     # you'll add audit trail logic here
│   └── agents/                 # agent pattern module
└── tests/                      # you'll add tests here
```

By the end of today, this repo - under *your* GitHub account, is yours to keep and show off.
