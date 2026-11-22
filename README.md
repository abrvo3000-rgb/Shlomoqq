# AI ONE 2.0 — iPhone-only PWA

Static app in Hebrew. No Python, server process, API keys, or build tools required.

## Publish from an iPhone with GitHub Pages
1. In Safari sign in to https://github.com and create a new PUBLIC repository, e.g. `ai-one` (public hosting means code is public; don't put secrets in the files).
2. Upload **the four files** `index.html`, `manifest.webmanifest`, `icon.svg`, `sw.js` to the **repository root** using Add file → Upload files → Commit changes. On iPhone, unzip this project in the Files app first. GitHub mobile web may require requesting Desktop Website.
3. Open repository Settings → Pages → Build and deployment → Deploy from a branch; select `main` and `/ (root)` and save.
4. After publishing, open `https://YOUR_USERNAME.github.io/ai-one/` in Safari. Share → Add to Home Screen → Add.
5. For updates, upload replacement files and commit; Safari may take time to refresh cached resources.

GitHub Pages is a public static site. Data (products/tasks) is stored only in Safari localStorage on that device, not in GitHub. Export backups from the app. Deleting website data or changing the site's URL can remove access to stored data.

## What works
- Responsive RTL Hebrew interface, installable web app, offline shell after first HTTPS load.
- Local task manager, product pricing/profit per unit, JSON export/import.
- Image/video prompt builder (does not generate media).
- Links to external Google/Wikipedia search.
- Compose/copy an instruction and open ChatGPT separately (does not automatically submit prompts).

## Not yet included
- Embedded LLM chat, actual image/video generation, unattended/background automation, cloud sync, push notifications, accounts.
- No API keys are stored in browser. Do not upload secrets or sensitive information.
