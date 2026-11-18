# FarsiYar (فارسی‌یار) — Improved Version

FarsiYar is a mobile-first, RTL language-learning web application teaching **Iranian Persian (Farsi)**—both **Conversational Tehrani (`ئاخاوتنی تاران`)** and **Formal Literary (`فەرمی و نووسین`)**—to **Kurdish Sorani (`کوردیی سۆرانی`)** speakers.

## What's New in this Improved Version
- **Better Design**: Refined dark theme, improved cards, smoother animations, better visual hierarchy and glass effects.
- **More Vocabulary**: Expanded from 48 to 60 carefully selected words/phrases across key categories (greetings, food, travel, market, verbs, shared words).
- **Polished UX**: Better mobile experience, improved active states and overall polish.
- Fully offline-first (PWA + Service Worker).

## Included Files
- `index.html`: Self-contained RTL application with all units, expanded vocabulary, sentence-building challenges, conversations, interactive quizzes, Web Speech API (`fa-IR`) + synthesized fallback audio, and `localStorage` persistence.
- `sw.js`: Offline-first Service Worker.
- `manifest.json`: PWA manifest for home-screen installation.
- `_headers` & `_redirects`: Cloudflare Pages routing and caching rules.

## Deploy to Cloudflare Pages (Free)

### Option 1: Direct Upload
1. Log in to the [Cloudflare Dashboard](https://dash.cloudflare.com/) → **Workers & Pages**.
2. Create application → Pages → Upload assets.
3. Name the project and upload the files.
4. Deploy. Your site will be live on `https://your-project.pages.dev`.

### Option 2: Wrangler CLI
```bash
npx wrangler pages deploy . --project-name=farsiyar
```

## GitHub Pages (optional)
You can also enable GitHub Pages on the `master` branch (root) if you prefer.
