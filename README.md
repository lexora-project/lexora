# Lexora

Lexora is an AI-assisted multilingual reading layer for the browser. It helps users understand selected web content in context without leaving the page.

**Fewer surfaces, deeper trust.**

## Status

The latest public release is **v0.19.2 — Stability and recovery**, published on Chrome Web Store on October 15, 2026. See the [installation guide](https://lexora.sh/install).

This repository is a **public project hub** and does not contain the full extension source code. The capabilities below describe the publicly available v0.19.2 release.

## Translation Modes in v0.19.2

- **On-device Translation** — Chrome’s built-in Translator API with browser-managed language packs. Supported prepared language pairs can translate offline. Availability depends on Chrome, the document, and the language pair. Failures never silently select a remote translation provider.
- **Google Translate** — online translation; the default mode. No Cloud AI key is required.
- **Cloud AI** — Gemini, OpenAI, and Anthropic with user-supplied API keys.

## New in v0.19.2

- Keep Cloud AI provider selection and saved credentials consistent.
- Recover stalled translation loading with bounded requests and retries that preserve the current selection.
- Restore reading panel and selection handling after browser back/forward navigation, including BFCache restores.
- Clear stale YouTube DualSubs text when subtitle timing, video, or language changes invalidate a cue.
- DualSubs controls follow the selected interface language across 10 existing locales; no translation target languages are added.

See [the changelog](CHANGELOG.md) for release details.

## Reading Capabilities

- **Selected-text Reading Panel** — translation and reading support in context, with assistance depending on the text, language, and settings.
- **Japanese reading and pronunciation** — furigana and pronunciation support when available.
- **Wikipedia/Wikidata** — reference context and cross-language article lookup.
- **YouTube DualSubs** — original and translated captions on supported videos, using YouTube’s service separately from Reading Panel translation.
- **Notebook** — explicitly save selections locally, revisit them in Options, or export Markdown. Saving is unavailable in incognito tabs.
- **Translation and privacy settings** — configure translation mode, automatic reading features, pronunciation, reference lookups, and subtitles. API keys use the chosen local or session storage and authenticate provider requests directly.

On-device Translation applies to translation text. Other enabled reading features can make separate network requests, including automatic workflows. Review the [Privacy Policy](https://lexora.sh/privacy) for details and offline limitations.

## Links

| Resource | URL |
|----------|-----|
| Website | [lexora.sh](https://lexora.sh) |
| Help | [Reading guide](https://lexora.sh/help) |
| Changelog | [Release notes](https://lexora.sh/changelog) |
| Privacy Policy | [Privacy](https://lexora.sh/privacy) |
| Support | [Support](https://lexora.sh/support) |
| Security | [Security](https://lexora.sh/security) |
| Install | [Installation guide](https://lexora.sh/install) |

## Source Code

This repository is a public project hub for Chrome Web Store reviewers, testers, and users. The full extension source code is not published here at this stage of development.
