# LCS Resolve AI — Support Demo

An AI-powered customer support briefing tool for Rent Manager support teams. Built with vanilla HTML/JS and the Anthropic Claude API.

## What it does

- Shows incoming customer call queue with account details
- Generates an AI briefing for each customer — predicts why they're calling
- Cross-matches open support tickets against recent hotfixes
- Chat window lets agents ask follow-up questions about any customer

## How to use (deployed version)

1. Open the live URL
2. Paste your own Anthropic API key in the top bar (`sk-ant-...`)
3. Click any customer in the sidebar
4. Read the AI briefing, browse tickets/hotfixes, and chat

Your API key is used only in your browser session and never stored.

## Deploy to Netlify (free)

### Option A — Drag and drop (quickest)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the entire `lcs-demo` folder onto the page
3. Done — you get a live URL

### Option B — Connect GitHub (auto-deploys on push)
1. Sign up at [netlify.com](https://netlify.com)
2. Click **Add new site → Import from Git**
3. Select this repository
4. Leave build settings blank
5. Click **Deploy**

> The `netlify/functions/claude.js` proxy is required because browsers can't call the Anthropic API directly (CORS). Netlify handles this automatically when you deploy the full folder.

## Tech stack

- Vanilla HTML + CSS + JavaScript (no build step)
- Anthropic Claude API (`claude-sonnet-4-20250514`)
- Netlify Functions (serverless proxy)

## Note

This is a demo with hardcoded mock data. In production you'd connect to a real Rent Manager database and ticketing system.
