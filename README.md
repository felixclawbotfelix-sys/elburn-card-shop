# Elburn Card Shop Website

Mobile-first single-page site for Elburn Card Shop.

## Stack
- Pure HTML/CSS/JS — no framework, no build step
- Hosted on Cloudflare Pages (free tier)
- Optional custom domain (elburnCardShop.com or similar, ~$10/yr on Cloudflare)

## Sections
- Buy / Sell / Trade hero
- Product categories
- Visit Us (hours, address, phone, map)
- Hobby Blog (starter posts, expandable)
- AI Hobby Bot (Anthropic Claude Haiku)
- Social links
- Footer

## AI Bot
The bot uses Anthropic Claude Haiku via browser-side API call.
Set your API key in the HTML before deploying:
  window.ANTHROPIC_API_KEY = 'YOUR_KEY_HERE'
Or use a Cloudflare Worker proxy to keep the key server-side (recommended for production).

## Deploy to Cloudflare Pages
1. Push this folder to a GitHub repo
2. Go to Cloudflare Pages → Create project → Connect GitHub repo
3. No build command needed — output directory = /
4. Done — live at yourproject.pages.dev

## Add Custom Domain
1. Buy domain at Cloudflare Registrar (~$10/yr)
2. In Cloudflare Pages → Custom domains → Add domain
3. DNS auto-configures
