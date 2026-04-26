# LCS Rent Manager AI Support Demo

AI-powered support console demo for Rent Manager.

## Setup

### 1. Push to GitHub
Push this repo to GitHub as-is.

### 2. Connect to Netlify
1. Go to app.netlify.com
2. Click **Add new site** → **Import an existing project**
3. Connect your GitHub account
4. Select this repository
5. Build settings are auto-detected from `netlify.toml`
6. Click **Deploy**

### 3. Add the API Key (one time only)
1. In Netlify dashboard → your site → **Site configuration** → **Environment variables**
2. Click **Add a variable**
3. Key: `ANTHROPIC_API_KEY`
4. Value: your `sk-ant-api03-...` key
5. Click **Save**
6. Go to **Deploys** → click **Trigger deploy** → **Deploy site**

Done. Share the Netlify URL — no API key entry needed for users.
