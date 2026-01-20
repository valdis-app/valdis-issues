# Valdis — Issue Tracker

This repository is **only** for bug reports and feature requests for **Valdis**.
Valdis is **closed-source** — no code lives here.

## Quick links

- **Report a bug / request a feature:** https://github.com/valdis-app/valdis/issues/new/choose
- **Browse existing issues:** https://github.com/valdis-app/valdis/issues
- **Website / Download:** https://valdis.app
- **Support:** https://valdis.app/faq
- **Privacy:** https://valdis.app/privacy

## How to open an issue

1) Sign in to GitHub.
2) Open the new issue chooser: https://github.com/valdis-app/valdis/issues/new/choose
3) Pick **Bug report** or **Feature request**, fill out the template, and submit.

## Before you file an issue

1) Search existing issues first.
2) If it’s a **crash / bug**, include:
   - Device + OS version (macOS/iOS + version)
   - Diagnostics (includes Valdis version/build + system info)
      - **macOS:** menu bar → **Valdis → About Valdis** → **Copy diagnostics**
      - **iOS:** Valdis → **Settings → About** → **Copy diagnostics**
   - Steps to reproduce
   - Expected vs actual behavior
   - Screenshots / screen recording (if helpful)
   - Logs **only if you’re comfortable sharing them** (Valdis is privacy-first; logs don’t include chat/prompt content
     or secrets)
## Debug logging

Valdis includes an optional Debug logging mode. When enabled, you can copy recent app logs to include in bug reports.

- **macOS:** Menu bar → **Valdis → About Valdis** → **Debug logging**
- **iOS:** Valdis → **Settings → About** → **Debug logging**
- Restart the app after changing the setting.
- After restart, use **Copy logs** (toolbar button) to copy recent logs.
- Logs exclude sensitive content (prompts, context, message text, and secrets).

### Screenshots

| macOS: Enable                                                                         | iOS: Enable                                                                         |
|---------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| <img src="images/mac-debug-mode.png" alt="macOS Debug logging toggle" height="400" /> | <img src="images/ios-debug-mode.png" alt="iOS Debug logging toggle" height="400" /> |

| macOS: Copy logs                                                                        | iOS: Copy logs                                                                        |
|-----------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------|
| <img src="images/mac-logs-copy-button.png" alt="macOS Copy logs button" height="400" /> | <img src="images/ios-logs-copy-button.png" alt="iOS Copy logs button" height="400" /> |



## Reset flags (macOS)

If Valdis behaves strangely after an update (or when asked by a maintainer), you can start from a clean state using command‑line reset flags.

⚠️ **These actions are destructive and cannot be undone.** Only use them if you understand what will be deleted.

- `--reset-settings` — resets app settings
- `--reset-data` — resets local app data
- `--reset-history` — clears chat history

### Run (recommended)

```bash
open -a Valdis --args --reset-data --reset-settings --reset-history
```

### Run (direct binary)

```bash
/Applications/Valdis.app/Contents/MacOS/Valdis --reset-data --reset-settings --reset-history
```

## What to report here

✅ Bugs, UX issues, performance problems  
✅ Feature requests & product ideas  
✅ Docs / website issues

## What not to post

❌ Secrets (tokens, keys), private conversation content, personal data

## Security

If you believe you found a security issue, **do not** open a public issue.
Email: security@valdis.app


## Thanks ❤️

- **[Ollama](https://github.com/ollama/ollama)** — local LLM runtime
- **[WhisperKit](https://github.com/argmaxinc/WhisperKit)** (by **Argmax**) — on-device speech-to-text
- **[Vapor](https://github.com/vapor/vapor)** — WebSocket server backend on macOS
- **[Ready Player Me](https://readyplayer.me/)** — avatars
- **[Swift Markdown UI](https://github.com/gonzalezreal/swift-markdown-ui)** — Markdown rendering
