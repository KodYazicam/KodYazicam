<div align="center">

<img src="https://raw.githubusercontent.com/KodYazicam/svgforge/main/examples/banner.svg" alt="KodYazicam" width="100%"/>

<br/>

**Developer tools I actually use.** Local CLIs, no telemetry, attribution license. Clone the repo — nothing is published to npm or PyPI.

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-KodYazicam-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/KodYazicam)
[![Instagram](https://img.shields.io/badge/Instagram-kodyazicam-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/kodyazicam)

</div>

---

## About

Türkiye. I write small tools that remove a daily annoyance (packing a repo for an LLM, linting `.env`, catching a webhook, drawing a README SVG without a CDN), then I use them.

English first. TR: kod yazıyorum, sistem kuruyorum, çözüm üretiyorum.

What you can click in this org is TypeScript CLIs, a Python FastAPI inspector, and Discord bots. Nest / Mongo / Redis show up at work; they are not in these public repos.

## Open source tools

Free under **[KYAL-1.0](https://github.com/KodYazicam/ctxpack/blob/main/LICENSE)** (use and fork, keep the credit). Not OSI-approved.

| Repo | What it does | Run |
| --- | --- | --- |
| **[ctxpack](https://github.com/KodYazicam/ctxpack)** | Pack a codebase into LLM-ready context. Nested gitignore, token budget, secret redaction. | `git clone` → `npm ci && npm run build` → `node dist/cli.js . -o prompt.md` |
| **[envsentinel](https://github.com/KodYazicam/envsentinel)** | Lint `.env` against a schema. Scan secrets. Emit `.env.example` and `env.d.ts`. | `git clone` → `npm ci && npm run build` → `node dist/cli.js check` |
| **[sparkcord](https://github.com/KodYazicam/sparkcord)** | File-based Discord.js v14 framework. Slash + prefix, cooldowns, permissions. | `git clone` → `npm ci && npm run build` → `node dist/cli.js init my-bot` |
| **[hookyard](https://github.com/KodYazicam/hookyard)** | Local webhook inspector. Catch, verify GitHub/Stripe/Slack, replay without SSRF. | `git clone` → `pip install -e .` → `hookyard --port 4242` |
| **[svgforge](https://github.com/KodYazicam/svgforge)** | Generate README SVGs locally. Banners, stats, skill bars, terminals. | `git clone` → `npm ci && npm run build` → `node dist/cli.js banner --title x -o banner.svg` |

Also shipping: [discord-music-panel](https://github.com/KodYazicam/discord-music-panel) (self-hosted, encrypts bot tokens) · [Stribog-Bot](https://github.com/KodYazicam/Stribog-Bot) (moderation + per-guild economy) · [awesome-developer-portfolios](https://github.com/KodYazicam/awesome-developer-portfolios)

Banners in those READMEs are **files in the repo**, generated with svgforge — not capsule-render / github-readme-stats CDNs.

## Stack (evidenced here)

TypeScript · Node 20+ · Vitest · FastAPI · Discord.js v14 · SQLite · Docker · GitHub Actions

## Contact

- GitHub: [KodYazicam](https://github.com/KodYazicam)
- Instagram: [kodyazicam](https://instagram.com/kodyazicam)
- Security: private advisory on the relevant repo (see each `SECURITY.md`)

<sub>KodYazicam — tools first, badges second.</sub>
