# Resume Tailor (Open Source)

**Resume Tailor** is a local-first job application assistant that turns your base resume + a target job posting into a full application package in minutes.

You provide:
- the role details
- your master resume
- optional priorities for this application

It generates:
- tailored resume
- tailored cover letter
- LinkedIn connection note
- LinkedIn recruiter message
- suggested outreach titles (who to contact)

No account required. No project backend required.

---

## What This Tool Solves

Most applicants lose time rewriting the same materials for every role. Resume Tailor compresses the repetitive work so you can focus on final judgment:
- choosing the right roles
- editing for truth and accuracy
- personalizing with your own voice

---

## Core Features

- **5-step guided workflow** from setup to final outreach assets
- **Provider flexibility**: Claude, ChatGPT, Gemini, or local Ollama
- **Fit analysis step** before generation (go/no-go scoring)
- **Comms Center output tabs** for each asset type
- **Outreach title suggestions** with direct LinkedIn search links
- **Local history** stored in your browser for quick iteration

---

## Quick Start

1. Download or clone this repository.
2. Open `index.html` in a browser.
3. Select an AI provider and enter your API key (or use Ollama locally).
4. Work through Steps 1–5 in order.

For best compatibility, run from a local server (especially for Ollama and browser security restrictions).

---

## Workflow Guide (Step by Step)

### Step 1 — Your Secret Identity Key

Choose your provider and add your key:
- Claude (Anthropic)
- ChatGPT (OpenAI)
- Gemini (Google)
- Ollama (local)

If you use Ollama, follow the built-in setup guide and keep the local service running.

### Step 2 — What Is the Job?

Add job context:
- company
- role title
- full job description

Optional: use URL fetch to auto-fill fields from a posting page.

### Step 3 — Your Resume

Paste your **master** resume (recommended) or upload a file.

Best practice:
- open your resume in PDF/Word
- Select All, Copy, Paste into Step 3

This usually gives cleaner text than relying on PDF extraction.

### Step 4 — The Score

Run fit analysis before generating assets.

You get:
- 0–100 fit score
- strengths
- gaps

Use this as a filter: decide whether to tailor deeply, lightly, or move on.

### Step 5 — Comms Center

Generate and review:
- tailored resume
- cover letter
- LinkedIn connection note
- recruiter/hiring manager message
- who-to-reach-out-to title list

Each section includes quick copy/download actions where applicable.

---

## Screenshots

### Main Workflow
![Main screen](docs/images/main-screen.png)

### Fit Analysis
![Fit analysis](docs/images/fit-analysis.png)

### Scoring View
![Scoring](docs/images/scoring.png)

### Generated Outputs
![Generated outputs](docs/images/generated-output.png)

---

## Privacy & Data Handling

Resume Tailor does **not** use a project-owned backend to store your resume or job content.

When you run analysis/generation, your prompts go directly from your browser to the provider you selected:
- Anthropic (Claude)
- OpenAI (ChatGPT)
- Google (Gemini)
- or your own local Ollama host

Local history is saved in your browser storage on your device.

---

## Provider Recommendations

| Provider | Best for | Notes |
|---|---|---|
| Claude | Strong writing quality and nuanced tone | Great default for high-polish outputs |
| ChatGPT (`gpt-4o`) | Balanced quality/speed | Reliable structured outputs |
| Gemini (`gemini-1.5-flash`) | Fast iteration and budget-friendly usage | Good for repeated drafts |
| Ollama (local) | Privacy-first local generation | Requires local setup and compatible model |

If unsure, start with Claude or ChatGPT for first-pass quality, then iterate.

---

## Troubleshooting

### I get API errors or retries
- Verify key format and available provider credits
- Retry after short delay (temporary provider overload can happen)
- Try a different provider if needed

### URL fetch fails
Some career pages block extraction/proxies.  
Fallback: copy the description manually into Step 2.

### PDF upload looks messy
This can happen due to PDF layout encoding.  
Best workaround: open PDF/Word, Select All, copy/paste plain text into Step 3.

---

## Docs

- Setup guide: `docs/SETUP.md`
- API key guide: `docs/API_KEYS.md`

---

## Contributing

Contributions are welcome for:
- prompt quality improvements
- UI/UX polish
- provider/model compatibility
- documentation clarity

Open an issue or PR with a clear summary and before/after behavior.

---

## Attribution

Built by [Michael Findling](https://linkedin.com/in/michaelfindling)  
Website: [gtmstack.pro](https://gtmstack.pro)