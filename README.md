# Paid Media Intelligence

A 7-division AI report powered by Claude that generates comprehensive paid media strategy reports. Built for Railway.app deployment.

---

## Analysis Divisions

| Stage | Division | Specialty |
|-------|----------|-----------|
| 01 | Account Health Review | Structural evaluation, campaign efficiency, competitive positioning |
| 02 | Data Integrity & Attribution Audit | Tag management, conversion accuracy, cross-platform attribution |
| 03 | Search Intent & Query Performance | Intent classification, waste elimination, keyword opportunities |
| 04 | Campaign Architecture & Growth Strategy | Account structure, bidding framework, budget allocation |
| 05 | Creative Performance & Messaging Strategy | Ad copy evaluation, RSA architecture, creative testing |
| 06 | Social Media Advertising Strategy | Full-funnel social, audience engineering, platform execution |
| 07 | Programmatic Media & Display Buying | Display strategy, DSP planning, partner media, ABM targeting |

---

## Deploy to Railway

### Step 1 — Fork or Clone
```bash
git clone https://github.com/yourusername/paid-media-intelligence.git
cd paid-media-intelligence
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
| `CLAUDE_API_KEY` | Anthropic Claude API key — get from console.anthropic.com |
| `LS_API_KEY` | LemonSqueezy API key — get from app.lemonsqueezy.com → Settings → API |
| `PORT` | Auto-set by Railway, do not set manually |

---

## File Structure

```
paid-media-intelligence/
├── index.html          # Frontend UI
├── server.js           # Backend + all 7 division prompts
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
