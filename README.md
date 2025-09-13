Prospective Memory Trainer

Daily reality‑check cues for lucid dreaming (MILD). Private by default, works offline.

Live app

- https://ra13s.github.io/prospective-memory-trainer/

What it does

- Generates 4 random everyday cues to practice reality checks.
- Add your own cues; keep or exclude the built‑in defaults.
- Remembers today’s list so it doesn’t change on refresh.
- Works fully offline; nothing is uploaded anywhere.
- English/Estonian UI with a language selector (auto‑detects too).

How to use

- Open the link above and click Generate (it auto‑generates if there are ≥ 4 cues).
- Add your own cues under “My items”. Toggle “Include default items” if you want only your list.
- Import/Export lets you save or load your personal cues as JSON.

Offline use

- Click the link above, then Save Page As (or download the repo ZIP).
- Ensure `index.html` and `targets.js` are in the same folder; double‑click `index.html`.
- Everything works without internet; your data stays in this browser.

Privacy

- Your custom cues and today’s list are stored only in your browser’s localStorage.
- No analytics, no trackers, no uploads — completely local.

For developers

- System defaults: `targets.js` exports `window.PM_DEFAULTS = [{ id, en, et }]`.
- UI and content are static; publish these two files anywhere (e.g., GitHub Pages).
