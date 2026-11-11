<div align="center">
  <img src="./assets/banner.svg" alt="Batuhan — local-first developer tools for the AI era" width="100%" />
  <img src="./assets/pills.svg" alt="TypeScript, Python, MCP, offline-first, Apache-2.0" width="100%" />
</div>

# Hi, I'm Batuhan

I build **local-first developer tools** for the AI era: CLIs and MCP servers that keep source code, secrets, and webhooks on your machine.

I care about tools that are **small, offline by default, secure by design, and documented like products** — not demos.

**English** · [Türkçe](./README.tr.md) · [Website](https://kodyazicam.github.io/KodYazicam/)

[Flagship tools](#flagship-tools) · [Why local-first](#why-local-first) · [Also building](#also-building) · [Toolbox](#toolbox) · [How I work](#how-i-work) · [Contact](#contact)

---

## Flagship tools

| Project | What it does | Install |
| --- | --- | --- |
| **[ctxpack](https://github.com/KodYazicam/ctxpack)** | Packs a repository into an LLM-ready prompt. Respects `.gitignore`, budgets tokens, redacts secrets. Ships an MCP server. | `npm i -g @kodyazicam/ctxpack` |
| **[envsentinel](https://github.com/KodYazicam/envsentinel)** | Validates `.env` against a JSON schema, scans for leaked secrets, and generates `.env.example` plus TypeScript types. | `npm i -g @kodyazicam/envsentinel` |
| **[svgforge](https://github.com/KodYazicam/svgforge)** | Generates README banners, cards, and stats as committed SVG files. 32 card types, 22 themes, no render service. | `npm i -g @kodyazicam/svgforge` |
| **[hookyard](https://github.com/KodYazicam/hookyard)** | Inspects, verifies, and replays webhooks locally. GitHub, Stripe, Slack, and Discord signatures; SSRF-safe replay. | [Source install](https://github.com/KodYazicam/hookyard#install) |

All four are **Apache-2.0**, **offline-first**, and **scriptable**. `ctxpack`, `envsentinel`, and `hookyard` also expose MCP servers for AI agents.

> **In progress:** a single `kodyaz` entry point that exposes the suite as one CLI and one MCP server. See the [suite architecture](./docs/SUITE.md).

<div align="center">
  <img src="./assets/terminal.svg" alt="Terminal: ctxpack, envsentinel, hookyard, svgforge" width="100%" />
</div>

---

## Why local-first?

- **Your code stays yours.** No upload, no account, no telemetry.
- **Works when the network does not.** Air-gapped machines, CI runners, locked-down laptops.
- **Composable by design.** Plain files in, plain files out. Every tool is scriptable.
- **Agent-ready.** MCP lets Claude, Cursor, and other clients call the tools directly.

---

## Also building

| Project | Status | What it is |
| --- | --- | --- |
| **[sparkcord](https://github.com/KodYazicam/sparkcord)** | beta | File-based Discord.js v14 framework with slash + prefix commands, cooldowns, permissions, and a validator. |
| **[LogYazicam](https://github.com/KodYazicam/LogYazicam)** | active | Self-hosted Discord logging bot with per-guild routing, filters, 88 event keys, 24 groups, 18 locales, and per-event overrides. |
| **[discord-music-panel](https://github.com/KodYazicam/discord-music-panel)** | stable | Self-hosted multi-bot Discord music panel with a React dashboard. |
| **[awesome-developer-portfolios](https://github.com/KodYazicam/awesome-developer-portfolios)** | community | Curated list of developer portfolios. MIT, contributions welcome. |

---

## Contribution stats

As of 2026-11-11. Counts are authored by me across all repositories; historical work is included.

**Pull requests:** 188 total · 172 merged

| # | Repository | PRs |
| ---: | --- | ---: |
| 1 | [LogYazicam](https://github.com/KodYazicam/LogYazicam) | 49 |
| 2 | [KY-GamePlayer](https://github.com/KodYazicam/KY-GamePlayer) | 18 |
| 3 | [wabot-aq](https://github.com/KodYazicam/wabot-aq) | 17 |
| 4 | [libredb/libredb-studio](https://github.com/libredb/libredb-studio) | 16 |
| 5= | [KodYazicam](https://github.com/KodYazicam/KodYazicam), [svgforge](https://github.com/KodYazicam/svgforge) | 13 each |

<sub>Also at 10: `discord-music-panel`, `hookyard`; at 8: `Stribog-Bot`; at 6: `ctxpack`, `envsentinel`; at 4: `sparkcord`; at 3: `libredb/libredb-database`; at 2: `awesome-developer-portfolios`; 13 further PRs in upstream repositories.</sub>

**Issues:** 145 total · 4 open

| # | Repository | Issues |
| ---: | --- | ---: |
| 1 | [LogYazicam](https://github.com/KodYazicam/LogYazicam) | 53 |
| 2 | [wabot-aq](https://github.com/KodYazicam/wabot-aq) | 17 |
| 3 | [KY-GamePlayer](https://github.com/KodYazicam/KY-GamePlayer) | 16 |
| 4 | [svgforge](https://github.com/KodYazicam/svgforge) | 12 |
| 5 | [KodYazicam](https://github.com/KodYazicam/KodYazicam) | 10 |

<sub>Also at 9: `hookyard`; at 8: `discord-music-panel`; at 6: `Stribog-Bot`; at 4: `ctxpack`, `envsentinel`, `sparkcord`; at 1: `awesome-developer-portfolios` and `libredb/libredb-studio`.</sub>

<sub>Open: <a href="https://github.com/KodYazicam/sparkcord/issues/8">sparkcord#8</a> (assigned to <a href="https://github.com/bongurishi">@bongurishi</a>), <a href="https://github.com/KodYazicam/discord-music-panel/issues/23">discord-music-panel#23</a>, <a href="https://github.com/KodYazicam/Stribog-Bot/issues/19">Stribog-Bot#19</a>, <a href="https://github.com/KodYazicam/svgforge/issues/32">svgforge#32</a>.</sub>


---

## Toolbox

- **Languages:** TypeScript · JavaScript · Python · SQL
- **Backend:** Node.js · FastAPI · SQLite · REST · WebSockets
- **Frontend:** React · Tailwind CSS · PySide6
- **Tooling:** Docker · GitHub Actions · pytest · Vitest · Linux

Currently deepening: PostgreSQL, Redis, and production observability.

---

## How I work

- **Docs are part of the product.** Every repo ships install steps, examples, limits, and troubleshooting.
- **Security is a feature.** Secret redaction, HMAC verification, SSRF guards, and local-only defaults.
- **Small surfaces.** Prefer one sharp CLI over a platform that does everything.
- **No fake metrics.** If something is not published, the README says so.
- **Responsible automation.** Read the [policy](./ETHICS.md).

<div align="center">
  <img src="./assets/quote.svg" alt="Ship tools that work offline." width="100%" />
</div>

---

## Contributing

The fastest way in is a `good first issue`:

- [ctxpack](https://github.com/KodYazicam/ctxpack/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
- [envsentinel](https://github.com/KodYazicam/envsentinel/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
- [svgforge](https://github.com/KodYazicam/svgforge/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
- [sparkcord](https://github.com/KodYazicam/sparkcord/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

## Contact

- Open an issue or discussion in the relevant repository.
- For security reports, use the `SECURITY.md` in that repository.
- GitHub: [@KodYazicam](https://github.com/KodYazicam)
- Website: [kodyazicam.github.io/KodYazicam](https://kodyazicam.github.io/KodYazicam/)

<sub>Profile assets are generated locally with <a href="https://github.com/KodYazicam/svgforge">svgforge</a> · Content licensed <a href="./LICENSE">CC-BY-4.0</a>.</sub>
