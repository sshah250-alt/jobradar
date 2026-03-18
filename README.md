# JobRadar v3 — Suman Shah

AI-powered job scanner for Supply Chain & Procurement roles in California.

## Deploy in 5 minutes (Vercel — Free)

### Step 1 — Push to GitHub
1. Create a new GitHub repo (e.g. `jobradar`)
2. Upload all 3 files: `index.html`, `api/claude.js`, `vercel.json`

### Step 2 — Deploy to Vercel
1. Go to [vercel.com](https://vercel.com) → Sign up free with GitHub
2. Click **"Add New Project"** → Import your `jobradar` repo
3. Click **Deploy** (no build settings needed)

### Step 3 — Add your API Key (secret, never exposed)
1. In Vercel dashboard → Your project → **Settings → Environment Variables**
2. Add:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** `sk-ant-...` (your key from console.anthropic.com)
3. Click **Save** → Go to **Deployments** → **Redeploy**

### Step 4 — Use it!
Your app is live at `https://your-project.vercel.app`
Open it in any browser, anywhere — no setup needed.

## How it works
- `index.html` — The frontend UI
- `api/claude.js` — Serverless function that calls Anthropic API (key never exposed to browser)
- `vercel.json` — Routes `/claude` to the serverless function

## Security
- API key stored as Vercel environment variable (encrypted, never in code)
- No database, no user data stored
