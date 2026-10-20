# Changelog

## v0.20.2 — Cloud AI Timeout Reliability (2026-10-20)

Lexora v0.20.2 is published and publicly available on Chrome Web Store as of October 20, 2026.

- Cloud AI requests have more time to complete, with timeouts adapted to selection length.
- Timeout failures are not cached, so a manual retry starts a fresh request after the previous attempt settles.
- Provider selection and privacy safeguards are preserved; no automatic timeout retries or silent provider fallback.

## v0.20.1 — Reading Tools & Multilingual Toolbar (2026-10-18)

Lexora v0.20.1 is published and publicly available on the Chrome Web Store. Public availability was confirmed on October 18, 2026. This update brings together all improvements since v0.19.3.

- New Word Length Highlighter in Toolbar → Lexora → Reading Tools: highlight words with 1–30 characters on the current webpage, replace or clear highlights, and keep them during normal reading and supported content changes. Matching stays local without sending page text to an AI provider.
- The toolbar follows Settings → Interface language across all 10 existing interface languages, including Reading Tools, YouTube controls, statuses, and errors, while preserving relevant popup state when the language changes.
- Improved YouTube DualSubs compatibility and reliability while preserving video navigation and subtitle behavior.
- Updated OpenAI Cloud AI translation to GPT-6 Luna (gpt-6-luna), replacing GPT-5 mini and removing the automatic GPT-4.1 mini fallback. Model access failures are shown instead of silently switching models.
- Updated Anthropic translation to Claude Haiku 5.5 (claude-haiku-5-5); Gemini 3.5 Flash-Lite remains unchanged. Existing provider selections and API keys are preserved, and translation attribution uses the response model when supplied.
- Improved Cloud AI instruction isolation so selected questions and commands are translated as text rather than followed.

## v0.19.3 — Reliability and consistency (2026-10-16)

Lexora v0.19.3 is published and publicly available on the Chrome Web Store. Public availability was confirmed on October 16, 2026.

- More reliable Notebook saves, duplicate detection across websites, and bookmark synchronization between tabs.
- Fixed incorrect cached translations for long selections that share the same beginning.
- More reliable settings persistence across contexts, with clear errors when a save fails.
- Improved YouTube DualSubs loading and language changes. Temporary rate limits can still require a short wait before retrying.
- Restored reliable Wikipedia references when enabled.
- Improved selection handling in embedded frames after the background worker restarts.
- Completed Notebook labels, filters, notices, and controls across all ten interface languages.
- Removed verified obsolete extension code and unused website content.

## v0.19.2 — Stability and recovery (2026-10-15)

Lexora v0.19.2 was published publicly on the Chrome Web Store on October 15, 2026.

- Keep Cloud AI provider selection and saved credentials consistent.
- Recover stalled translation loading with bounded requests and retries that preserve the current selection.
- Restore reading panel and selection handling after browser back/forward navigation, including BFCache restores.
- Clear stale YouTube DualSubs text when subtitle timing, video, or language changes invalidate a cue.
- DualSubs controls follow the selected interface language across 10 existing locales; no translation target languages are added.


## v0.19.1 — Popup and update awareness (2026-10-10)

Lexora v0.19.1 was published on the Chrome Web Store on October 10, 2026.

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
