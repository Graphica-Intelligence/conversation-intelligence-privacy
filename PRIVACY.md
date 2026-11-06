# Privacy Policy — Conversation Intelligence (HyperKode)

**Last updated:** November 6, 2026

This Privacy Policy describes how the **Conversation Intelligence** Chrome extension (the “Extension”) handles information as part of its local-first AI conversation intelligence features.

## 1) What the Extension does
Conversation Intelligence runs on supported chat sites (ChatGPT and Claude) to build a visual minimap of the conversation and provide features such as navigation, search, starring, summaries, and export.

## 2) Information the Extension processes

### A. On-page content (ChatGPT / Claude conversation content)
When you are on a supported page, the Extension reads and analyzes the page content (e.g., prompts and responses) **to render the minimap, enable navigation, run search, compute word frequency/similarity, and optionally generate summaries**. This processing occurs **in your browser**.

### B. User settings and local state (stored by the Extension)
The Extension stores certain information locally using Chrome’s extension storage (the Extension requests the `storage` permission).

Examples may include:
- Display preferences (themes, modes, toggles)
- Feature enable/disable choices (e.g., semantic features, overlays)
- Local UI state
- User markers (e.g., stars) and related metadata (if enabled)
- Optional local caches used for performance (e.g., summary/similarity cache)

### C. Local layout diagnostics
When the Extension detects that recognizable messages are missing from its map, it
shows a warning. **Copy diagnostic** copies only the supported site name, extension
version and message counts. It does not include message text, conversation titles,
message identifiers or the page URL. Diagnostics are not uploaded automatically.

### D. Exported data (only when you choose to export)
If you use an export feature, the Extension generates an export artifact in your browser. Exports are initiated by you and produced locally.

### E. Imported conversation library
JSON exports you choose to import are read and stored locally in this browser
profile. The library does not upload imports, contact AI providers, download remote
attachments, or sync imported conversations with the original service. External
links in messages open only when you choose to follow them.

You can remove imported conversations from the library. Removing an import does not
change its source file or original chat. Clearing extension data or uninstalling the
Extension removes the locally stored library. Keep your original export as a backup.

## 3) What the Extension does **not** collect by default
- The Extension does **not** sell personal information.
- The Extension does **not** use your data for advertising.
- The Extension does **not** transmit your chat content to HyperKode servers.

## 4) Network access and third parties

### Default behavior: no off-device sharing
By default, the Extension does not send your chat content to any external server.

### Optional AI integrations
The Extension may optionally connect to:

- a **local** AI service running on your computer, such as an LLM server listening on `http://localhost:11434/` or `http://127.0.0.1:11434/`
- supported **remote BYOK providers**, currently including OpenAI and Anthropic endpoints, if you explicitly enable and configure them

AI is **off by default** on a fresh installation and is configured in Labs. Remote
AI can send the relevant conversation text, requests and derived results directly
to the chosen provider. That provider's own terms and privacy policy apply. Provider
API keys are kept in browser-session extension storage and can be cleared in the
Extension; they are not included in diagnostics or sent to HyperKode.

These connections are only used to power optional AI features such as summaries, search assistance, embeddings, or related analysis.

- Local AI connections, if used, are **loopback (on-device)**.
- Remote BYOK requests are only made when you choose to enable and configure a supported provider.
- The Extension does not send your chat content to HyperKode servers by default.

## 5) Permissions explained (plain English)
The Extension requests:
- **`storage`**: to save your settings and local state (such as preferences, stars, and feature caches).
- **Host permissions for `localhost:11434` / `127.0.0.1:11434`**: to allow optional connections to a local AI service on your machine.
- **Host permissions for supported remote provider endpoints**: to allow optional direct BYOK connections to providers you choose to configure.

The Extension runs on specific sites (ChatGPT and Claude) via content scripts in order to render the minimap and related UI features.

## 6) Data retention
- Locally stored settings/state persist until you clear them (by clearing extension data in Chrome) or uninstall the Extension.
- If you enable local AI features, any local caching remains on your device and follows the same retention behavior.

## 7) Security
The Extension is designed to minimize data collection and keep processing on-device. You control the Extension’s stored data through Chrome’s extension management settings.

## 8) Your choices and controls
You can:
- Disable or uninstall the Extension at any time
- Clear extension storage via Chrome settings
- Use features like summaries only if you choose to enable them, whether through a local AI service or a supported remote BYOK provider

## 9) Changes to this policy
We may update this policy as the Extension evolves. The “Last updated” date will be revised accordingly. Material changes will be reflected in the Chrome Web Store listing and/or Extension UI where appropriate.

## 10) Limited use
The Extension's use of user data adheres to the Chrome Web Store User Data Policy,
including the Limited Use requirements. Data is used only for the disclosed
conversation navigation, organization, export and user-enabled analysis features.
It is not sold or used for advertising, unrelated profiling, creditworthiness or
lending decisions.

## 11) Contact
**Developer:** HyperKode (Carlos Enrique Ortiz) © 2026  
**Website:** https://hyperkode.com  
**Support:** enrique.ortiz+hk@gmail.com
