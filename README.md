<img width="688" height="384" alt="image" src="https://github.com/user-attachments/assets/89927afd-33bc-497d-8873-2da0078541cd" />

# Resume Tailor (Open Source)

Resume Tailor helps job seekers go from **job post → tailored application package** in one focused workflow.

It is built to reduce repetitive rewriting, improve message alignment, and give you cleaner first drafts fast.

---

## Who This Is For

- Job seekers who want stronger, role-specific applications without starting from scratch every time
- Career switchers translating existing experience into a new function or industry
- Professionals applying to multiple roles and needing a faster, repeatable workflow
- People who want practical AI assistance but still keep final editorial control

---

## What You Get

From one target role and your base resume, Resume Tailor generates:

- Tailored resume
- Tailored cover letter
- LinkedIn connection note
- LinkedIn recruiter/hiring manager message
- Suggested outreach titles (who to find and contact)

You can copy everything immediately and download key documents when needed.

---

## Why People Use It

Most job applications fail on speed or consistency:
- Resume not aligned to the role language
- Cover letter too generic
- Outreach started too late (or not at all)

Resume Tailor gives you a practical system:
1. Qualify the role with a fit score
2. Tailor your materials in one pass
3. Leave with both assets and outreach angles

---

## Quick Start

1. Download or clone this repository.
2. Open `index.html` in your browser.
3. Choose an AI provider and add your key (or use Ollama locally).
4. Run Steps 1–5 in sequence.

Tip: for best browser compatibility, use a local server instead of opening with `file://`.

---

## The 5-Step Workflow

### Step 1 — Your Secret Identity Key
- Select provider: Claude, ChatGPT, Gemini, or Ollama
- Add your API key (or local Ollama host/model)
- Confirm provider readiness before moving on

### Step 2 — What Is the Job?
- Add company, role title, and full job description
- Optional: use URL fetch to auto-fill fields
- Confirm details are accurate before scoring

### Step 3 — Your Resume
- Paste your master resume (recommended)
- You can upload PDF/Word/TXT, but direct paste is usually cleaner
- Best practical workflow: open resume in PDF/Word, Select All, Copy, Paste

### Step 4 — The Score
- Run fit analysis before generating final materials
- Get:
  - 0–100 fit score
  - top strengths
  - likely gaps
- Use this as your go/no-go filter

### Step 5 — Comms Center
- Review all output tabs in one place
- Copy, edit, and export as needed
- Use the outreach tab to quickly identify titles worth contacting on LinkedIn

---

## Screenshots

### Main Workflow
![Main workflow](docs/images/main-screen.png)

### Fit Analysis
![Fit analysis](docs/images/fit-analysis.png)

### Generated Outputs
![Generated outputs](docs/images/generated-output.png)

---

## Privacy & Data Handling

Resume Tailor does **not** run a project-owned backend that stores your resume or job content.

When you click analyze/generate, your prompt is sent directly from your browser to the provider you selected:

- Anthropic (Claude)
- OpenAI (ChatGPT)
- Google (Gemini)
- Local Ollama (if configured)

History is saved in your browser storage on your own device.

---

## Provider Guidance

| Provider | Best for | Notes |
|---|---|---|
| Claude | High-quality tone and nuanced rewrite quality | Great default for polished first drafts |
| ChatGPT (`gpt-4o`) | Balanced speed + consistency | Reliable for structured outputs |
| Gemini (`gemini-1.5-flash`) | Fast iteration and lower-cost loops | Strong for frequent revision |
| Ollama (local) | Local-first privacy workflows | Requires setup + compatible local model |

If you are unsure, start with Claude or ChatGPT, then optimize for speed/cost.

---

## Troubleshooting

### API call errors / retries
- Verify key format and account credits
- Retry after a short delay (temporary provider overload is common)
- Switch providers if needed

### URL fetch does not work
Some sites block extraction/proxy flows.  
Fallback: copy/paste the job description directly in Step 2.

### Uploaded PDF text looks messy
PDF extraction can reorder content depending on the source file.  
Best workaround: copy/paste plain text from your resume into Step 3.

---

## Documentation

- Setup guide: `docs/SETUP.md`
- API key guide: `docs/API_KEYS.md`

---

## Contributing

Contributions are welcome, especially for:
- prompt quality
- UI/UX polish
- provider/model reliability
- onboarding and documentation clarity

Open an issue or PR with expected behavior, actual behavior, and screenshots when helpful.

---

## Attribution

Built by [Michael Findling](https://linkedin.com/in/michaelfindling)  
Website: [gtmstack.pro](https://gtmstack.pro)
