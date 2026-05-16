![wheel-of-heaven-banner](https://github.com/wheelofheaven/.github/blob/main/profile/static/wheel-of-heaven-banner.jpg)

# Wheel of Heaven

**Wheel of Heaven** explores the hypothesis that life on Earth was intelligently designed by an extraterrestrial civilization known as the Elohim. Drawing from ancient astronaut theory, Raëlian scriptures, and biblical exegesis, this multilingual knowledge base presents encyclopedic content, cosmic chronology, sacred texts, and curated resources.

## Explore

| | |
|---|---|
| [**Knowledge Base**](https://www.wheelofheaven.world) | Browse 1,251 pages across wiki entries, timeline, library, and more |
| [**Wiki**](https://www.wheelofheaven.world/wiki/) | Encyclopedia of key terms, concepts, and figures |
| [**Timeline**](https://www.wheelofheaven.world/timeline/) | The Great Year — 12 precessional ages spanning 26,000 years |
| [**Library**](https://www.wheelofheaven.world/library/) | Sacred texts with reading tools, bookmarks, and highlights |
| [**Resources**](https://www.wheelofheaven.world/resources/) | Curated books, documentaries, and websites |

## Languages

Available in 9 languages: English, Deutsch, Español, Français, 日本語, 한국어, Русский, 简体中文, 繁體中文

## White Paper

The [original white paper](https://github.com/wheelofheaven/.github/blob/main/profile/WHITEPAPER.md) (2018) tells the story of the Great Year — how the precessional cycle frames the Elohim's creation of life on Earth across cosmic ages.

## Connect

- [Telegram](https://t.me/wheelofheaven) — Community chat
- [X (Twitter)](https://x.com/wheelofheaven) — Updates
- [Open Collective](https://opencollective.com/wheelofheaven) — Support the project

---

## For Developers

### Web Properties

| Site | Description |
|------|-------------|
| [www.wheelofheaven.world](https://www.wheelofheaven.world) | Main knowledge base |
| [api.wheelofheaven.world](https://api.wheelofheaven.world) | JSON API |
| [assets.wheelofheaven.world](https://assets.wheelofheaven.world) | Image CDN |

### Repositories

**Sites**
- [www.wheelofheaven.world](https://github.com/wheelofheaven/www.wheelofheaven.io) — Main Zola static site
- [api.wheelofheaven.world](https://github.com/wheelofheaven/api.wheelofheaven.io) — JSON API endpoints
- [bifrost](https://github.com/wheelofheaven/bifrost) — Zola theme

**Content & Data**
- [data-content](https://github.com/wheelofheaven/data-content) — Markdown content (1,330 files)
- [data-library](https://github.com/wheelofheaven/data-library) — Book catalog and chapters
- [data-images](https://github.com/wheelofheaven/data-images) — Image processing pipeline

**Documentation**
- [docs](https://github.com/wheelofheaven/docs) — Technical documentation

### Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    Cloudflare Pages                          │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐          │
│  │     www     │  │     api     │  │   assets    │          │
│  │  (Zola)     │  │  (Zola)     │  │   (CDN)     │          │
│  └──────┬──────┘  └──────┬──────┘  └─────────────┘          │
└─────────┼────────────────┼──────────────────────────────────┘
          │                │
    ┌─────┴────────────────┴─────┐
    │      Shared Submodules      │
    │  ┌─────────┐ ┌───────────┐ │
    │  │ bifrost │ │data-content│ │
    │  │ (theme) │ │(markdown)  │ │
    │  └─────────┘ └───────────┘ │
    └─────────────────────────────┘
```

### Tech Stack

- **Generator:** [Zola](https://www.getzola.org/) (Rust)
- **Hosting:** [Cloudflare Pages](https://pages.cloudflare.com/)
- **Theme:** Bifrost (custom)
- **Task Runner:** [mise](https://mise.jdx.dev/)

### Contributing

See [docs](https://github.com/wheelofheaven/docs) for setup guides, content authoring, and translation workflows.

---

*Open source under CC0-1.0 (Public Domain)*
