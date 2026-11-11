<div align="center">
  <img src="./assets/banner.svg" alt="Batuhan — yapay zeka çağı için local-first geliştirici araçları" width="100%" />
  <img src="./assets/pills.svg" alt="TypeScript, Python, MCP, offline-first, Apache-2.0" width="100%" />
</div>

# Merhaba, ben Batuhan

Yapay zeka çağı için **local-first geliştirici araçları** yazıyorum: kaynak kodun, secret'ların ve webhook'ların makinenin dışına çıkmayan CLI'lar ve MCP sunucuları.

Önem verdiğim şey **küçük, varsayılan olarak çevrimdışı çalışan, güvenli ve ürün gibi dokümante edilmiş** araçlar — demo değil.

[English](./README.md) · **Türkçe** · [Website](https://kodyazicam.github.io/KodYazicam/)

[Öne çıkan araçlar](#öne-çıkan-araçlar) · [Neden local-first?](#neden-local-first) · [Diğer projeler](#diğer-projeler) · [Araç kutusu](#araç-kutusu) · [Nasıl çalışıyorum](#nasıl-çalışıyorum) · [İletişim](#i̇letişim)

---

## Öne çıkan araçlar

| Proje | Ne yapar? | Kurulum |
| --- | --- | --- |
| **[ctxpack](https://github.com/KodYazicam/ctxpack)** | Bir repoyu LLM'e hazır prompt'a paketler. `.gitignore`'a uyar, token bütçesi koyar, secret'ları redakte eder. MCP sunucusu içerir. | `npm i -g @kodyazicam/ctxpack` |
| **[envsentinel](https://github.com/KodYazicam/envsentinel)** | `.env` dosyasını JSON şemasına göre doğrular, sızan secret'ları tarar, `.env.example` ve TypeScript tipleri üretir. | `npm i -g @kodyazicam/envsentinel` |
| **[svgforge](https://github.com/KodYazicam/svgforge)** | README banner, kart ve istatistiklerini commit edilen SVG dosyaları olarak üretir. 32 kart tipi, 22 tema, render servisi yok. | `npm i -g @kodyazicam/svgforge` |
| **[hookyard](https://github.com/KodYazicam/hookyard)** | Webhook'ları yerelde inceler, doğrular ve yeniden oynatır. GitHub, Stripe, Slack ve Discord imzaları; SSRF-safe replay. | [Kaynaktan kurulum](https://github.com/KodYazicam/hookyard#install) |

Dördü de **Apache-2.0**, **offline-first** ve **scriptable**. `ctxpack`, `envsentinel` ve `hookyard` ayrıca AI ajanları için MCP sunucusu sunar.

> **Üzerinde çalışıyorum:** Tüm araçları tek bir CLI ve tek bir MCP sunucusu olarak açan `kodyaz` giriş noktası. [Suite mimarisi](./docs/SUITE.md).

<div align="center">
  <img src="./assets/terminal.svg" alt="Terminal: ctxpack, envsentinel, hookyard, svgforge" width="100%" />
</div>

---

## Neden local-first?

- **Kodun sende kalır.** Upload yok, hesap yok, telemetri yok.
- **Ağ yokken de çalışır.** Air-gapped makineler, CI runner'ları, kısıtlı laptoplar.
- **Tasarımı gereği birleştirilebilir.** Girdi dosya, çıktı dosya. Her araç script'lenebilir.
- **Ajanlara hazır.** MCP sayesinde Claude, Cursor ve diğer istemciler araçları doğrudan çağırabilir.

---

## Diğer projeler

| Proje | Durum | Ne yapar? |
| --- | --- | --- |
| **[sparkcord](https://github.com/KodYazicam/sparkcord)** | beta | Dosya tabanlı Discord.js v14 framework'ü: slash + prefix komutlar, cooldown, yetki ve validator. |
| **[LogYazicam](https://github.com/KodYazicam/LogYazicam)** | active | Sunucu bazlı yönlendirme, filtreler, 88 event anahtarı, 24 grup, 18 dil ve event bazlı override'lar sunan self-hosted Discord log botu. |
| **[discord-music-panel](https://github.com/KodYazicam/discord-music-panel)** | stable | React paneli olan self-hosted çoklu bot Discord müzik paneli. |
| **[awesome-developer-portfolios](https://github.com/KodYazicam/awesome-developer-portfolios)** | community | Derlenmiş developer portfolyo listesi. MIT, katkıya açık. |

---

## Katkı istatistikleri

2026-11-12 itibarıyla. Sayılar tüm repolarda benim açtığım PR ve issue'ları sayar; eski çalışmalar dahildir.

**Pull request:** 196 toplam · 180 merge

| # | Repo | PR |
| ---: | --- | ---: |
| 1 | [LogYazicam](https://github.com/KodYazicam/LogYazicam) | 53 |
| 2 | [KY-GamePlayer](https://github.com/KodYazicam/KY-GamePlayer) | 18 |
| 3= | [wabot-aq](https://github.com/KodYazicam/wabot-aq), [KodYazicam](https://github.com/KodYazicam/KodYazicam) | 17'şer |
| 5 | [libredb/libredb-studio](https://github.com/libredb/libredb-studio) | 16 |

<sub>13'er adetle: `svgforge`; 10'ar adetle: `discord-music-panel`, `hookyard`; 8'er adetle: `Stribog-Bot`; 6'şar adetle: `ctxpack`, `envsentinel`; 4'er adetle: `sparkcord`; 3'er adetle: `libredb/libredb-database`; 2'şer adetle: `awesome-developer-portfolios`; upstream repolarda 13 PR daha.</sub>

**Issue:** 153 toplam · 4 açık

| # | Repo | Issue |
| ---: | --- | ---: |
| 1 | [LogYazicam](https://github.com/KodYazicam/LogYazicam) | 57 |
| 2 | [wabot-aq](https://github.com/KodYazicam/wabot-aq) | 17 |
| 3 | [KY-GamePlayer](https://github.com/KodYazicam/KY-GamePlayer) | 16 |
| 4 | [KodYazicam](https://github.com/KodYazicam/KodYazicam) | 14 |
| 5 | [svgforge](https://github.com/KodYazicam/svgforge) | 12 |

<sub>9'ar adetle: `hookyard`; 8'er adetle: `discord-music-panel`; 6'şar adetle: `Stribog-Bot`; 4'er adetle: `ctxpack`, `envsentinel`, `sparkcord`; 1'er adetle: `awesome-developer-portfolios` ve `libredb/libredb-studio`.</sub>

<sub>Açık: <a href="https://github.com/KodYazicam/sparkcord/issues/8">sparkcord#8</a> (<a href="https://github.com/bongurishi">@bongurishi</a>'ye atandı), <a href="https://github.com/KodYazicam/discord-music-panel/issues/23">discord-music-panel#23</a>, <a href="https://github.com/KodYazicam/Stribog-Bot/issues/19">Stribog-Bot#19</a>, <a href="https://github.com/KodYazicam/svgforge/issues/32">svgforge#32</a>.</sub>


---

## Araç kutusu

- **Diller:** TypeScript · JavaScript · Python · SQL
- **Backend:** Node.js · FastAPI · SQLite · REST · WebSockets
- **Frontend:** React · Tailwind CSS · PySide6
- **Araçlar:** Docker · GitHub Actions · pytest · Vitest · Linux

Şu anda derinleştiğim alanlar: PostgreSQL, Redis ve production observability.

---

## Nasıl çalışıyorum

- **Dokümantasyon ürünün parçasıdır.** Her repoda kurulum, örnek, limit ve troubleshooting var.
- **Güvenlik bir özelliktir.** Secret redaksiyonu, HMAC doğrulama, SSRF koruması ve local-only varsayılanlar.
- **Küçük yüzey.** Her şeyi yapan bir platform yerine tek ve keskin bir CLI.
- **Sahte metrik yok.** Bir şey yayınlanmadıysa README bunu açıkça söyler.
- **Sorumlu otomasyon.** [Politikayı oku](./ETHICS.md).

<div align="center">
  <img src="./assets/quote.svg" alt="Ship tools that work offline." width="100%" />
</div>

---

## Katkı

En hızlı başlangıç `good first issue` etiketli konular:

- [ctxpack](https://github.com/KodYazicam/ctxpack/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
- [envsentinel](https://github.com/KodYazicam/envsentinel/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
- [svgforge](https://github.com/KodYazicam/svgforge/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
- [sparkcord](https://github.com/KodYazicam/sparkcord/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

## İletişim

- İlgili repoda issue veya discussion açabilirsin.
- Güvenlik bildirimleri için o repodaki `SECURITY.md` dosyasını kullan.
- GitHub: [@KodYazicam](https://github.com/KodYazicam)
- Website: [kodyazicam.github.io/KodYazicam](https://kodyazicam.github.io/KodYazicam/)

<sub>Profil görselleri <a href="https://github.com/KodYazicam/svgforge">svgforge</a> ile yerelde üretilir.</sub>

<sub>İçerik <a href="./LICENSE">CC-BY-4.0</a> ile lisanslıdır.</sub>
