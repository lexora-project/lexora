# Privacy Summary

The approved canonical Privacy Policy is published at **[lexora.sh/privacy](https://lexora.sh/privacy)**. This curated summary describes v0.19.0, publicly available on Chrome Web Store as confirmed on October 9, 2026. Consult the canonical policy for complete disclosures.

## Translation and Reading Data

Lexora processes selected text and bounded reading context to provide translation, reading assistance, and pronunciation. The three translation modes have different data paths:

- **On-device Translation** uses Chrome’s built-in Translator API and browser-managed language packs. Supported prepared language pairs can translate offline. Translation text stays on-device, and failures never silently select a remote translation provider. Browser, document, and language-pair availability vary; language-pack preparation may require a download.
- **Google Translate**, the default, sends selected text and language information directly to Google’s online translation service. It does not require or load Cloud AI credentials.
- **Cloud AI** sends selected text and bounded relevant context directly to Gemini, OpenAI, or Anthropic over HTTPS using your API keys. The preferred provider is tried first; other supported providers with saved keys may be tried. Cloud AI failures do not switch to Google Translate. Test connection sends a fixed test phrase to the selected cloud provider.

Wikipedia/Wikidata reference lookups, pronunciation, and Japanese reading may send separate requests independently of translation mode. Some reference lookup translation paths use Google Translate. Automatic activation and pronunciation can trigger requests when enabled. On-device Translation does not make these other features offline.

YouTube DualSubs is enabled by default and can automatically request original and translated captions from YouTube’s timedtext service, including video/track identifiers, language choices, and existing YouTube session cookies. Caption translation uses YouTube independently of Reading Panel mode and Cloud AI keys. It can be disabled in settings or player controls.

## Local Storage and Controls

Settings and Notebook entries remain in local extension storage. Notebook saves are explicit; entries can be deleted or exported as Markdown. Incognito saves are blocked. Exported files remain under your control.

Cloud AI keys are stored separately in persistent local storage (the default) or temporary session storage, according to your choice. They authenticate requests directly to providers and are not sent to Lexora. Extension storage is not an encrypted password vault. Keys can be cleared in settings.

Review automatic activation, pronunciation, Wikipedia, DualSubs, and redaction settings alongside translation mode. Redaction is limited and cannot guarantee removal of every sensitive detail. Providers may retain requests under their own terms; Lexora cannot promise zero retention or no model training by a provider.

Lexora does not require a Lexora account or sell user data. Cloud providers may require their own accounts and billing.

## Questions

See the [canonical policy](https://lexora.sh/privacy) or contact [lexora.dev@proton.me](mailto:lexora.dev@proton.me).
