![wheel-of-heaven-banner](https://github.com/wheelofheaven/.github/blob/main/profile/static/wheel-of-heaven-banner.jpg)

# Wheel of Heaven

**Wheel of Heaven** explores the hypothesis that life on Earth was intelligently designed by an extraterrestrial civilization known as the Elohim. This multilingual knowledge base presents encyclopedic content, cosmic chronology, sacred texts, and curated resources.

## Web Properties

| Site | Description |
|------|-------------|
| [www.wheelofheaven.io](https://www.wheelofheaven.io) | Main knowledge base (1,251 pages, 9 languages) |
| [api.wheelofheaven.io](https://api.wheelofheaven.io) | JSON API for programmatic access |
| [assets.wheelofheaven.io](https://assets.wheelofheaven.io) | Image CDN |

## Repositories

### Core Sites
| Repository | Purpose |
|------------|---------|
| [www.wheelofheaven.io](https://github.com/wheelofheaven/www.wheelofheaven.io) | Main Zola static site |
| [api.wheelofheaven.io](https://github.com/wheelofheaven/api.wheelofheaven.io) | JSON API endpoints |
| [bifrost](https://github.com/wheelofheaven/bifrost) | Zola theme (templates, SCSS, JS) |

### Content & Data
| Repository | Purpose |
|------------|---------|
| [data-content](https://github.com/wheelofheaven/data-content) | Markdown content (1,330 files) |
| [data-library](https://github.com/wheelofheaven/data-library) | Book catalog and chapters |
| [data-images](https://github.com/wheelofheaven/data-images) | Image processing pipeline |

### Documentation
| Repository | Purpose |
|------------|---------|
| [docs](https://github.com/wheelofheaven/docs) | Technical documentation |
| [.claude](https://github.com/wheelofheaven/.claude) | AI assistant context |

## Technology Stack

- **Static Site Generator:** [Zola](https://www.getzola.org/) (Rust-based)
- **Hosting:** Cloudflare Pages (edge deployment)
- **Theme:** Bifrost (custom multilingual theme)
- **Task Runner:** [mise](https://mise.jdx.dev/)

## Architecture

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

## Content Sections

- **Wiki** — Encyclopedia of terms and concepts
- **Timeline** — Precessional ages and cosmic chronology
- **Library** — Sacred texts with study tools
- **Resources** — Curated books, videos, websites
- **Essentials** — Quick reference guides
- **Explainers** — In-depth articles

## Languages

English (default), Deutsch, Español, Français, 日本語, 한국어, Русский, 简体中文, 繁體中文

## White Paper

The [original white paper](https://github.com/wheelofheaven/.github/blob/main/profile/WHITEPAPER.md) (2018) synthesizes the narrative foundation exploring the precessional cycle as a timeline for Raëlian cosmology.

## Contributing

We welcome contributions! See our [documentation](https://github.com/wheelofheaven/docs) for:
- Content authoring guidelines
- Local development setup
- Translation workflows

## Support

- [Open Collective](https://opencollective.com/wheelofheaven) — Financial support
- [GitHub Issues](https://github.com/wheelofheaven/www.wheelofheaven.io/issues) — Bug reports and suggestions

## Connect

- [Telegram](https://t.me/wheelofheaven)
- [X (Twitter)](https://x.com/wheelofheaven)
- [GitHub](https://github.com/wheelofheaven)

---

*Built with [Zola](https://www.getzola.org/), hosted on [Cloudflare Pages](https://pages.cloudflare.com/), open source under CC0-1.0.*
