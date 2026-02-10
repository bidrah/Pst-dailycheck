# Pst-dailycheck

A single-page daily inspection checklist web app (`noki.html`).

## Run locally

Because this is a static HTML app, you can run it with any static file server.

### Option 1: Python (quickest)
```bash
cd /workspace/Pst-dailycheck
python3 -m http.server 8000
```
Then open:
- `http://localhost:8000/noki.html`

### Option 2: Open directly in browser
You can also open `noki.html` directly, but using a local server is recommended.

## Deploy

This project is static, so it can be deployed to any static hosting service.

### A) GitHub Pages
1. Push this repo to GitHub.
2. In GitHub repo settings, open **Pages**.
3. Set **Source** to deploy from your default branch (root folder).
4. Commit an `index.html` entry point (or rename `noki.html` to `index.html`) so Pages serves it by default.
5. Your app will be available at:
   - `https://<your-username>.github.io/<repo-name>/`

> If you keep the current filename, you can still access:
> `https://<your-username>.github.io/<repo-name>/noki.html`

### B) Netlify (drag-and-drop)
1. Go to Netlify and choose **Add new site** → **Deploy manually**.
2. Drag this project folder (or a zip of it).
3. Netlify publishes immediately and gives you a URL.

### C) Vercel
1. Import the GitHub repo into Vercel.
2. Framework preset: **Other**.
3. Build command: *(leave empty)*.
4. Output directory: `.` (root).
5. Deploy.

## Notes
- The app uses `localStorage`, so checklist data is stored per browser/device.
- No backend is required.
