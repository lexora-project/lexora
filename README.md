# Lexora

Lexora is an AI-assisted multilingual reading layer for the browser. It helps users understand selected web content in context without leaving the page.

**Fewer surfaces, deeper trust.**

## Status

The latest public release is **v0.20.1 — Reading Tools & Multilingual Toolbar**, published on Chrome Web Store on October 18, 2026. See the [installation guide](https://lexora.sh/install).

This repository is a **public project hub** and does not contain the full extension source code. The capabilities below describe the publicly available v0.20.1 release.

## Translation Modes in v0.20.1

- **On-device Translation** — Chrome’s built-in Translator API with browser-managed language packs. Supported prepared language pairs can translate offline. Availability depends on Chrome, the document, and the language pair. Failures never silently select a remote translation provider.
- **Google Translate** — online translation; the default mode. No Cloud AI key is required.
- **Cloud AI** — Gemini, OpenAI, and Anthropic with user-supplied API keys.

## New in v0.20.1

- New Word Length Highlighter in Toolbar → Lexora → Reading Tools: highlight words with 1–30 characters on the current webpage, replace or clear highlights, and keep them during normal reading and supported content changes. Matching stays local without sending page text to an AI provider.
- The toolbar follows Settings → Interface language across all 10 existing interface languages, including Reading Tools, YouTube controls, statuses, and errors, while preserving relevant popup state when the language changes.
- Improved YouTube DualSubs compatibility and reliability while preserving video navigation and subtitle behavior.
- Updated OpenAI Cloud AI translation to GPT-6 Luna (gpt-6-luna), replacing GPT-5 mini and removing the automatic GPT-4.1 mini fallback. Model access failures are shown instead of silently switching models.
- Updated Anthropic translation to Claude Haiku 5.5 (claude-haiku-5-5); Gemini 3.5 Flash-Lite remains unchanged. Existing provider selections and API keys are preserved, and translation attribution uses the response model when supplied.
- Improved Cloud AI instruction isolation so selected questions and commands are translated as text rather than followed.

See [the changelog](CHANGELOG.md) for release details.

## Reading Capabilities

- **Reading Tools** — Word Length Highlighter finds words with 1–30 characters locally on the current webpage. Open Toolbar → Lexora → Reading Tools to highlight, update, or clear matches.
- **Selected-text Reading Panel** — translation and reading support in context, with assistance depending on the text, language, and settings.
- **Japanese reading and pronunciation** — furigana and pronunciation support when available.
- **Wikipedia/Wikidata** — reference context and cross-language article lookup.
- **YouTube DualSubs** — original and translated captions on supported videos, using YouTube’s service separately from Reading Panel translation, with live appearance and positioning controls.
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
