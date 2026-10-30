# Installation

Full installation instructions are available at:

**[https://lexora.sh/install](https://lexora.sh/install)**

## Chrome Web Store (Primary Path)

Lexora v0.21.0 is the latest public release, published and publicly available on Chrome Web Store. Public availability was confirmed on October 30, 2026. Store installation remains the recommended path.

Open the official listing linked from [https://lexora.sh/install](https://lexora.sh/install), then select **Add to Chrome**. Developer Mode is not required.

## Choose a Translation Method

In the Reading Panel, choose **Machine Translation** (Google Translate, online and the default), **AI Translation** (OpenAI, Gemini, or Claude), or **On-device Translation** (Chrome Translator). For AI Translation, use the separate provider control and configure that provider’s API key in **Options → AI**, in your chosen local or session storage.

Switching to an AI provider first checks for its key in the chosen storage mode. A missing key shows provider-specific guidance and leaves the current route and result unchanged. Successful route changes translate the active selection again; leaving AI Translation retains the preferred AI provider. Requests use only the selected provider’s credential, and failures never silently switch providers, models, or methods. Machine Translation and On-device Translation do not use AI credentials.

For On-device Translation, follow the panel’s language-pack preparation guidance. Availability depends on Chrome, the document, and the language pair; supported prepared pairs can translate offline. Other enabled reading features may still make network requests. See the [Privacy Policy](https://lexora.sh/privacy).

## Reading Tools

Open the Lexora toolbar → **Lexora** tab → **Reading Tools**. Enter a character count from **1 to 30**, then press **Highlight**. Change the count and press **Highlight** to replace matches; use **Clear** when finished. Matching runs locally on supported webpage content. See the [reading guide](https://lexora.sh/help#reading-tools).

## Developer Mode / Manual Install (Contributors)

Manual installation via Chrome Developer Mode is for contributors and authorized testers working with development builds.

This path is not recommended for general users. Do not attempt to install unpacked extension files from unverified sources.

For access or instructions for an authorized development build, contact [lexora.dev@proton.me](mailto:lexora.dev@proton.me).

## Source Code

This repository does not contain the full extension source code. Do not attempt to build or install Lexora from this repository.
