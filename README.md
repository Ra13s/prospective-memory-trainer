Prospective Memory Trainer

Live

- GitHub Pages: https://ra13s.github.io/prospective-memory-trainer/

Overview

- Static, single-page app that picks 4 random targets from a flat list.
- Base list in `targets.js` (`window.PM_ITEMS = [ ... ]`) plus your custom items (saved in localStorage).
- No network, no server required. Fully offline capable.
- UI auto-detects language (English/Estonian) from the browser or `?lang=et|en`. Only UI is translated; item texts are not altered.
 - Language selector in the header lets users switch between English and Estonian. Choice is saved in localStorage.

Quick start

- Files: `index.html` and `targets.js`.
- Open the HTML directly (file://) — it auto-loads `targets.js` and auto-generates a list if there are ≥ 4 items.
- Click Generate to reshuffle anytime.
 - Change language via the selector (or URL `?lang=et|en`).

Edit targets

- Update `targets.js` and set `window.PM_ITEMS = [ "The next time I …", "…" ];`
- Add your own via the “My items” section; they persist in localStorage.
- Need at least 4 total (base + custom) to generate a list.
 - Today’s generated list is saved in localStorage and restored on reload. Click Generate to reshuffle for today (overwrites today’s saved list).

Import/Export custom items

- Export: Click Export to download `my_targets.json` with `{ schema: "pm-items-v1", userItems: ["..."] }`.
- Import: Click Import and select either a `["..."]` array or an object with `userItems`.
- Import merges with your existing custom items and de-duplicates.

Deploy to GitHub Pages

1. Create a new GitHub repo and add both files to the root.
2. Commit and push.
3. In the repo: Settings → Pages → Build and deployment → Source: `Deploy from a branch`.
4. Select branch `main` (or `master`), folder `/ (root)`, Save.
5. Wait for the page to publish; open the provided URL.

Suggested GitHub topics

- lucid-dreaming, reality-checks, prospective-memory, mild, dream-signs, offline, privacy, webapp

Notes

- Since `targets.js` is a plain script, it loads under `file://` and on GitHub Pages with no extra steps.
- Privacy: Data (custom items, today’s list) lives only in your browser’s localStorage and is never uploaded.
- Offline: You can download the two files and open `index.html` without any server.
