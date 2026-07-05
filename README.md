# Sankalp — Mission Prep Console

A single-page static site (`index.html`). No build step, no dependencies — just HTML/CSS/JS.

## Deploy to Vercel

### Option A — Drag & drop (no account setup, fastest)
1. Go to https://vercel.com/new
2. Log in (or sign up — free).
3. Drag this whole folder onto the page, or click to browse and select it.
4. Click **Deploy**. Vercel will detect it as a static site automatically.
5. You'll get a live URL like `https://your-project.vercel.app` in under a minute.

### Option B — Vercel CLI
1. Install the CLI (needs Node.js installed):
   ```
   npm install -g vercel
   ```
2. From inside this folder, run:
   ```
   vercel
   ```
3. Follow the prompts (log in / create account on first use, confirm project name, accept defaults — no build command needed).
4. For a permanent production URL:
   ```
   vercel --prod
   ```

### Option C — GitHub + Vercel (best if you'll keep editing it)
1. Create a new GitHub repo and push this folder to it:
   ```
   git init
   git add .
   git commit -m "Sankalp prep console"
   git branch -M main
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
2. Go to https://vercel.com/new, choose **Import Git Repository**, and select the repo.
3. Leave all build settings as default (Framework Preset: **Other**) and click **Deploy**.
4. Every future `git push` will auto-redeploy the site.

## Notes
- This app has no backend/database. Accounts, syllabus, and plans created by users live only in that browser's current session (in-memory) — refreshing clears them. Each user can use the **Export data** / **Import data** buttons in the app to save/restore their own progress as a JSON file.
- Nothing to configure in Vercel's project settings — no environment variables, no build command, no output directory overrides needed.
