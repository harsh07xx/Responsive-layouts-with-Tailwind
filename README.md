# Signal House — Digital Product Studio

A single-page marketing site for Signal House, a digital product studio offering brand, product design, web development, and growth engineering.

**[View live demo →](https://YOUR-USERNAME.github.io/signal-house-site/)** *(update after enabling GitHub Pages)*

---

## ✨ Features

- Animated hero with cursor-following spotlight grid
- Scramble-in text effect on headings
- Scroll-triggered reveal animations
- Animated count-up stats
- Infinite scrolling logo marquee
- Portfolio/work grid with hover-reveal logos
- Client-side contact form (demo only — see [Notes](#notes))
- Fully responsive, accessible focus states, and respects `prefers-reduced-motion`

## 🛠 Tech stack

| Layer  | Tool |
|--------|------|
| Markup | Static HTML |
| Styling | [Tailwind CSS](https://tailwindcss.com/) (via CDN) + custom CSS |
| Behavior | Vanilla JavaScript (no framework) |
| Fonts | Space Grotesk, Inter, IBM Plex Mono (Google Fonts) |
| Hosting | GitHub Pages |

## 📁 Project structure

```
.
├── index.html              # The entire site
├── 404.html                 # Custom not-found page (GitHub Pages)
├── robots.txt               # Search engine crawl rules
├── sitemap.xml               # Sitemap for search engines
├── package.json               # Dev-only scripts (no runtime deps)
├── .editorconfig               # Consistent formatting across editors
├── .github/
│   ├── workflows/deploy.yml     # Auto-deploy to GitHub Pages on push to main
│   └── ISSUE_TEMPLATE/bug_report.md
├── CONTRIBUTING.md
├── LICENSE
└── .gitignore
```

## 🚀 Getting started

Clone and run locally — no build step required:

```bash
git clone https://github.com/YOUR-USERNAME/signal-house-site.git
cd signal-house-site
npm start        # opens index.html on http://localhost:8000
```

Or just open `index.html` directly in your browser.

## 🌐 Deployment (GitHub Pages)

This repo includes a GitHub Actions workflow (`.github/workflows/deploy.yml`) that automatically deploys to GitHub Pages on every push to `main`.

**One-time setup:**
1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment → Source**, select **GitHub Actions**.
4. Push to `main` — the site deploys automatically. Check the **Actions** tab for progress.

Your site will be live at:
```
https://YOUR-USERNAME.github.io/signal-house-site/
```

## 🧭 Roadmap ideas

- [ ] Replace Tailwind CDN with a proper build (Tailwind CLI/PostCSS) for smaller CSS and no runtime warning
- [ ] Wire the contact form to a real backend (e.g. Formspree, Resend, or a serverless function)
- [ ] Add Open Graph / Twitter card meta tags for social sharing previews
- [ ] Add a favicon and app icons
- [ ] Split inline `<script>`/`<style>` into `/assets/js` and `/assets/css` if the project grows

## 📝 Notes

- **Tailwind via CDN**: convenient for prototyping, but not ideal for production — it ships the full framework unminified and warns in the console. Fine for a marketing page like this, but worth revisiting if the site grows.
- **Contact form**: currently client-side only — it shows a confirmation message but doesn't send data anywhere. Connect it to a form backend before relying on it for real leads.

## License

MIT — see [LICENSE](LICENSE).
