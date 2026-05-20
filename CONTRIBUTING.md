# Contributing to Wheel of Heaven

Thank you for your interest in contributing! This guide will help you get started.

## Ways to Contribute

### Content
- Fix typos or improve clarity
- Add missing translations
- Suggest new wiki entries or resources
- Report inaccuracies

### Code
- Fix bugs
- Improve accessibility
- Enhance performance
- Add features

### Other
- Report issues
- Suggest improvements
- Share the project

## Getting Started

### 1. Find Something to Work On

- Check [open issues](https://github.com/wheelofheaven/www.wheelofheaven.io/issues)
- Look for `good first issue` labels
- Or propose something new

### 2. Set Up Local Development

The fast path is the [Quickstart](https://docs.wheelofheaven.world/getting-started/quickstart/) — clone, build, preview in under five minutes. For the full dev environment (api, theme work, content-validation scripts), see [Local Setup](https://docs.wheelofheaven.world/contributing/dev/local-setup/).

### 3. Make Your Changes

**For content changes:**
- Edit files in the `data-content` repository
- Follow the per-content-type guides at
  [docs.wheelofheaven.world](https://docs.wheelofheaven.world/contributing/content/overview/)
  ([Wiki Entry](https://docs.wheelofheaven.world/contributing/content/wiki-entry/),
   [Article](https://docs.wheelofheaven.world/contributing/content/article/),
   [Newsroom Dispatch](https://docs.wheelofheaven.world/contributing/content/newsroom-dispatch/))
- Run validation: `python scripts/validate.py`

**For theme/code changes:**
- Edit files in `bifrost` (theme) or the site repos
- Follow existing code style
- Test locally with `mise run serve`

### 4. Submit a Pull Request

1. Fork the repository
2. Create a feature branch (`git checkout -b my-feature`)
3. Commit your changes
4. Push to your fork
5. Open a Pull Request

## Repository Guide

| Repo | What to Contribute |
|------|-------------------|
| [data-content](https://github.com/wheelofheaven/data-content) | Wiki entries, translations, resources |
| [bifrost](https://github.com/wheelofheaven/bifrost) | Templates, styles, JavaScript |
| [www.wheelofheaven.io](https://github.com/wheelofheaven/www.wheelofheaven.io) | Site configuration, static assets |
| [docs.wheelofheaven.world](https://github.com/wheelofheaven/docs.wheelofheaven.world) | Documentation improvements |

## Translation

We support 9 languages. To help translate:

1. Check coverage: `python scripts/i18n_dashboard.py`
2. Find missing translations (ko and zh-Hant need the most help)
3. Create translation files mirroring English structure
4. Use the [glossary](https://github.com/wheelofheaven/data-content/blob/main/i18n/glossary.json) for consistent terminology
5. Read the [Translations guide](https://docs.wheelofheaven.world/contributing/content/translations/) for per-language conventions

## Questions?

- Open a [GitHub Discussion](https://github.com/wheelofheaven/www.wheelofheaven.io/discussions)
- Join our [Telegram](https://t.me/wheelofheaven)

## License

By contributing, you agree that your contributions will be licensed under CC0-1.0 (Public Domain).
