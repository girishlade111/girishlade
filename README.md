# Girish Lade — Chatbot

> Single-file HTML chatbot UI — drop into any static host, no build step required.

A self-contained, browser-only chatbot client inspired by the ChatGPT interface. The whole experience (HTML, CSS, JavaScript, UI logic) lives in one `Chatbot` file at the repo root (~44 KB), so it can be served from anywhere a static file is reachable.

🔗 **Live repo:** <https://github.com/girishlade111/girishlade>
🔗 **Live demo:** <https://girishlade111.github.io/girishlade/>

## ✨ Features

- **Single-file deployment** — the entire chatbot is one HTML file, no build pipeline
- **ChatGPT-inspired UI** — green primary action (`#10a37f`) over a dark panel (`#343541` / `#202123`)
- **Responsive layout** — desktop and mobile-friendly viewport meta
- **Zero dependencies** — no `node_modules`, no CDN imports, no runtime fetches
- **GPL v3 licensed** — see `LICENSE`

## 🛠️ Tech stack

- HTML5
- CSS3 (custom properties, dark theme tokens)
- Vanilla JavaScript (no frameworks)
- Static hosting (GitHub Pages, Netlify, S3, local file://)

## 🚀 Getting started

```bash
# Option 1 — open directly
# Download "Chatbot" file, rename to "index.html", double-click to open

# Option 2 — serve locally
python -m http.server 8080
# Then open http://localhost:8080/Chatbot
```

> Tip: rename `Chatbot` → `index.html` if you want a cleaner URL when deploying to GitHub Pages or any static host.

## 📁 Project structure

```
.
├── Chatbot       # Single-file HTML chatbot UI (rename to index.html for hosting)
└── LICENSE       # GNU GPL v3
```

## 🎨 Theming

CSS custom properties at the top of the file:

| Token              | Default     | Purpose                  |
|--------------------|-------------|--------------------------|
| `--primary-color`  | `#10a37f`   | Send button, accents     |
| `--secondary-color`| `#343541`   | Sidebar / message bubble |
| `--dark-color`     | `#202123`   | Page background          |

Override any of these in your fork to re-skin the bot.

## 🤝 Contributing

Bug reports and pull requests are welcome. Because the whole UI lives in one HTML file, keep changes minimal and self-contained.

## 📜 License

GNU General Public License v3.0 — see [`LICENSE`](./LICENSE).

## 🌐 Deployment

Fully static — no build, no server, no API keys:

- **GitHub Pages** (live): `https://girishlade111.github.io/girishlade/` — deployed from the `gh-pages` branch, where the `Chatbot` file is published as `index.html`
- **Any static host**: copy the `Chatbot` file, rename it to `index.html`, upload to Netlify / Cloudflare Pages / S3 / any web server
- **Vercel/Cloudflare**: works as-is from any static export

## 🔧 Environment variables

None — the chatbot runs 100% in the browser with zero runtime configuration. No `.env` needed.

---

Built by Girish Lade · https://ladestack.in
