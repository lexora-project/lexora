# Changelog

## v0.19.0 — Browser-native Translation (2026-10-08)

Submitted to Chrome Web Store for review; public publication is not confirmed. The existing listing remains available. v0.18.4 is the last recorded published baseline.

- Added On-device Translation through Chrome’s built-in Translator API, with browser-managed language-pack preparation, progress, cancellation, and retry guidance in the Reading Panel.
- Three modes: On-device Translation, online Google Translate, and Cloud AI with user-supplied Gemini, OpenAI, or Anthropic keys. Supported prepared pairs can translate offline on-device; failures never silently select a remote translation provider.
- Improved Cloud AI connection handling and translation-mode persistence.
- Removed Ollama and custom endpoint support. Legacy endpoint selections migrate to On-device Translation.
- Existing Reading Panel, Japanese reading and pronunciation, Wikipedia/Wikidata, Notebook, and YouTube DualSubs retain their own settings and network behavior.

[Website release notes](https://lexora.sh/changelog) are available in English, Vietnamese, Japanese, and Korean for v0.19.0.

## v0.18.4 — Last recorded published baseline (2026-09-06)

Available publicly on the Chrome Web Store. This release improves reading-panel reliability and translation timeout handling.

Public release notes are available at [lexora.sh/changelog](https://lexora.sh/changelog).

## v0.18.0 — Historical preparation snapshot

*Public testing preparation release.*

The following records the preparation status when this public hub was created; it does not describe current availability:

> This version is being prepared for Chrome Web Store testing distribution. It represents the current state of Lexora as it goes through the review process.

---

*Earlier version history is not published in this repository.*
