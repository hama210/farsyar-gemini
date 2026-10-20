# FarsiYar (فارسی‌یار) — Cloudflare Pages Deployment Package

FarsiYar is a mobile-first, RTL language-learning web application teaching **Iranian Persian (Farsi)**—both **Conversational Tehrani (`ئاخاوتنی تاران`)** and **Formal Literary (`فەرمی و نووسین`)**—to **Kurdish Sorani (`کوردیی سۆرانی`)** speakers.

## Included Files
- `index.html`: Self-contained RTL application with all 6 beginner units, 48+ vocabulary cards, 12 sentence-building challenges, 5 multi-turn conversations, interactive quizzes, Web Speech API (`fa-IR`) + synthesized fallback audio, and `localStorage` persistence.
- `sw.js`: Offline-first Service Worker caching the core lessons and assets for offline access.
- `manifest.json`: PWA manifest for iOS/Android home-screen installation.
- `_headers` & `_redirects`: Cloudflare Pages routing and caching rules.

## Deploy to Cloudflare Pages (Free)

### Option 1: Direct Upload in Cloudflare Dashboard
1. Log in to the [Cloudflare Dashboard](https://dash.cloudflare.com/) and open **Workers & Pages**.
2. Click **Create application** -> **Pages** -> **Upload assets**.
3. Name your project `farsiyar` and upload the contents of this folder (`index.html`, `sw.js`, `manifest.json`, `_headers`, `_redirects`).
4. Click **Deploy site**. Your site will be live on `https://farsiyar.pages.dev`.

### Option 2: Deploy via Wrangler CLI
```bash
npx wrangler pages deploy . --project-name=farsiyar
```
