# LeadForge — AI Lead Generation Dashboard

A fully client-side lead generation app powered by Claude AI. Generate, enrich, and export leads from LinkedIn ads and other business sources — all from one dashboard.

## Features

- **✦ AI Generate** — Describe your ideal target (industry, job title, company size, geography) and Claude generates realistic, qualified leads
- **⌘ Paste Data** — Paste raw LinkedIn profiles, ad export snippets, or any unstructured contact data and Claude extracts leads automatically
- **⊞ Upload CSV** — Import any CSV (LinkedIn Ads export, Apollo, etc.) with intelligent column auto-mapping
- **✎ Manual Add** — Add individual leads by hand
- **⬇ Excel Export** — Export all leads to a formatted `.xlsx` file with a summary sheet

## Lead Fields Captured

| Field | Description |
|---|---|
| Name | Full name |
| Job Title | Role / position |
| Company | Company name |
| Industry | Sector / niche |
| Email | Professional email |
| Phone | With country code |
| LinkedIn URL | Profile link |
| Social / Website | Twitter, website, etc. |
| Source | Where the lead came from |
| Notes | AI-generated qualification notes |
| Date Added | Timestamp |

## Setup & Deployment

### GitHub Pages (Recommended)

1. Fork or create a new repo on GitHub
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages**
4. Set source to `main` branch, `/ (root)`
5. Your site will be live at `https://yourusername.github.io/your-repo/`

### Local Use

Just open `index.html` in any modern browser — no server needed.

## Usage

1. **Enter your Anthropic API key** at the top of the page  
   - Get one at [console.anthropic.com](https://console.anthropic.com)  
   - Your key is stored only in your browser's localStorage — never sent anywhere except the Anthropic API
2. Choose a generation method from the tabs
3. View and manage leads in the **Leads Table** tab
4. Click **Export Excel** to download your leads as `.xlsx`

## Notes

- Leads are saved in your browser's **localStorage** — they persist across sessions
- The app is 100% static — no backend, no database, no server costs
- The Anthropic API key is required only for AI Generate and Paste parsing features
- CSV upload works entirely client-side with no API key needed

## Tech Stack

- Vanilla HTML/CSS/JS (no framework)
- [SheetJS (xlsx)](https://sheetjs.com/) for Excel export
- [Anthropic Claude API](https://docs.anthropic.com) for AI generation & parsing
- Google Fonts (Syne + DM Mono)
