# Privacy Summary

The approved canonical Privacy Policy is published at **[lexora.sh/privacy](https://lexora.sh/privacy)**. This curated summary describes v0.21.0, published and publicly available on Chrome Web Store, with public availability confirmed on October 30, 2026. Two-Level Translation Routing separates method selection from AI-provider selection while retaining the data paths described below. Consult the canonical policy for complete disclosures.

## Translation and Reading Data

Lexora processes selected text and bounded reading context to provide translation, reading assistance, and pronunciation. The three translation methods have different data paths:

- **On-device Translation** uses Chrome Translator through Chrome’s built-in Translator API and browser-managed language packs. Supported prepared language pairs can translate offline. Translation text stays on-device, and failures never silently select a remote translation provider. Browser, document, and language-pair availability vary; language-pack preparation may require a download.
- **Machine Translation**, the default, uses Google Translate and sends selected text and language information directly to Google’s online translation service. It does not require or load AI credentials.
- **AI Translation** sends selected text and bounded relevant context directly to OpenAI, Gemini, or Claude (Anthropic) over HTTPS using your API keys. Only the selected provider and its key in the chosen storage mode are used. A missing key produces a configuration error; AI Translation does not silently switch providers, models, or translation methods, including Google Translate. Test connection sends a fixed test phrase to the selected cloud provider.

Before switching to an AI provider in the Reading Panel, Lexora checks for that provider’s key in the chosen local or session storage. If it is missing, guidance names the provider while the current route and result stay unchanged. Machine Translation and On-device Translation do not load AI credentials.

Wikipedia/Wikidata reference lookups, pronunciation, and Japanese reading may send separate requests independently of translation mode. Some reference lookup translation paths use Google Translate. Automatic activation and pronunciation can trigger requests when enabled. On-device Translation does not make these other features offline.

YouTube DualSubs is enabled by default and can automatically request original and translated captions from YouTube’s timedtext service, including video/track identifiers, language choices, and existing YouTube session cookies. Caption translation uses YouTube independently of Reading Panel mode and AI-provider keys. It can be disabled in settings or player controls.

## Local Storage and Controls

Settings and Notebook entries remain in local extension storage. Notebook saves are explicit; entries can be deleted or exported as Markdown. Incognito saves are blocked. Exported files remain under your control.

AI-provider keys are stored separately in persistent local storage (the default) or temporary session storage, according to your choice. They authenticate requests directly to providers and are not sent to Lexora. Extension storage is not an encrypted password vault. Keys can be cleared in settings.

Review automatic activation, pronunciation, Wikipedia, DualSubs, and redaction settings alongside translation mode. Redaction is limited and cannot guarantee removal of every sensitive detail. Providers may retain requests under their own terms; Lexora cannot promise zero retention or no model training by a provider.

Lexora does not require a Lexora account or sell user data. Cloud providers may require their own accounts and billing.

## Questions

See the [canonical policy](https://lexora.sh/privacy) or contact [lexora.dev@proton.me](mailto:lexora.dev@proton.me).
