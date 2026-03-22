# Paid Media Intelligence Pipeline

A 7-agent AI pipeline powered by Claude that generates comprehensive paid media strategy reports. Built for Railway.app deployment.

---

## Pipeline Agents

| Stage | Agent | Specialty |
|-------|-------|-----------|
| 01 | Paid Media Auditor | 200+ checkpoint account audit |
| 02 | Tracking & Measurement Specialist | GTM, GA4, CAPI, attribution |
| 03 | Search Query Analyst | Intent mapping, waste elimination |
| 04 | PPC Campaign Strategist | Account architecture, bidding strategy |
| 05 | Ad Creative Strategist | RSA, Meta creative, testing frameworks |
| 06 | Paid Social Strategist | Meta, LinkedIn, TikTok full-funnel |
| 07 | Programmatic & Display Buyer | GDN, DSP, ABM display |

---

## Deploy to Railway

### Step 1 — Fork or Clone
```bash
git clone https://github.com/yourusername/paid-media-pipeline.git
cd paid-media-pipeline
```

### Step 2 — Set Environment Variables in Railway
Go to your Railway project → Variables → Add:

```
CLAUDE_API_KEY=sk-ant-xxxxxxxxxxxxxxxx
LS_API_KEY=your_lemonsqueezy_api_key
```

### Step 3 — Deploy
```bash
# Option A: Connect GitHub repo to Railway (recommended)
# Option B: Railway CLI
npm install -g @railway/cli
railway login
railway init
railway up
```

---

## Environment Variables

| Variable | Description |
|----------|-------------|
| `CLAUDE_API_KEY` | Anthropic Claude API key |
| `LS_API_KEY` | LemonSqueezy API key for license validation |
| `PORT` | Auto-set by Railway |

---

## File Structure

```
paid-media-pipeline/
├── index.html          # Frontend UI
├── server.js           # Backend + all 7 agent prompts
├── package.json        # Node.js dependencies
├── railway.json        # Railway deployment config
├── .gitignore          # Git ignore rules
├── env.example         # Environment variable template
└── README.md           # This file
```

---

## Local Development

```bash
npm install
cp env.example .env
# Add your API keys to .env
node server.js
# Open http://localhost:3000
```

---

## License

Requires a valid LemonSqueezy license key to use.
Purchase at: https://bsfdataintelligence.lemonsqueezy.com
