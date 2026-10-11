# Changelog

## v0.19.1 — Popup and update awareness (2026-10-10)

Lexora v0.19.1 is the latest public release, published on the Chrome Web Store on October 10, 2026.

- Refined the toolbar popup to show the installed version, clear feature status, settings access, and compact secondary links.
- Genuine extension upgrades show a compact notice and a **NEW** toolbar badge until acknowledged. First installation, startup, popup reopening, and same-version reload do not create a new announcement.
- Opening the notice’s **What’s New** link or dismissing it acknowledges the installed version. Bundled release notes work offline.
- Improved keyboard tab navigation, focus indicators, accessible switches, and contextual YouTube player-control guidance.
- Chrome continues to manage extension package updates. This release adds no permissions, telemetry, automatic tabs, operating-system notifications, or custom downloader.

## v0.19.0 — Browser-native Translation (2026-10-08)

Lexora v0.19.0 was published and publicly available on the Chrome Web Store, with public availability confirmed on October 9, 2026.

- Added On-device Translation through Chrome’s built-in Translator API, with browser-managed language-pack preparation, progress, cancellation, and retry guidance in the Reading Panel.
- Three modes: On-device Translation, online Google Translate, and Cloud AI with user-supplied Gemini, OpenAI, or Anthropic keys. Supported prepared pairs can translate offline on-device; failures never silently select a remote translation provider.
- Improved Cloud AI connection handling and translation-mode persistence.
- Removed Ollama and custom endpoint support. Legacy endpoint selections migrate to On-device Translation.
- Existing Reading Panel, Japanese reading and pronunciation, Wikipedia/Wikidata, Notebook, and YouTube DualSubs retain their own settings and network behavior.

[Website release notes](https://lexora.sh/changelog) are available in English, Vietnamese, Japanese, and Korean for every release listed on the website.

## v0.18.4 — Historical public release (2026-09-06)

Available publicly on the Chrome Web Store. This release improves reading-panel reliability and translation timeout handling.

Public release notes are available at [lexora.sh/changelog](https://lexora.sh/changelog).

## v0.18.0 — Historical preparation snapshot

*Public testing preparation release.*

The following records the preparation status when this public hub was created; it does not describe current availability:

> This version is being prepared for Chrome Web Store testing distribution. It represents the current state of Lexora as it goes through the review process.

---

*Earlier version history is not published in this repository.*
