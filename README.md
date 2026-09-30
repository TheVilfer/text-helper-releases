# Text Helper

A macOS menu-bar app that fixes, formats and rewrites the text you select, in any app, with one shortcut. It runs on the Claude, ChatGPT or Grok subscription you already pay for. There are no API keys and no separate account.

This repository holds the releases, release notes and issue tracker. The app is free to use; its source code is not public.

## Install

1. Download the latest `TextHelper-<version>.dmg` from [Releases](../../releases/latest).
2. Open it, drag **Text Helper** into **Applications**, and launch it. It lives in the menu bar.
3. Grant **Accessibility** when asked (System Settings › Privacy & Security › Accessibility). The app needs it to read the selection and write the result back.
4. Connect a subscription in Settings › Accounts:
   - **Claude:** through the official `claude` CLI (Claude Code). The app shows the install command and a **Sign in with Claude** button. The CLI keeps its own login; the app never sees it.
   - **ChatGPT** or **Grok:** sign in from the app. Tokens stay in this Mac's Keychain.

Requires macOS 26 or later, on Apple silicon or Intel. Updates arrive by themselves (Sparkle, signed with the project's key); Settings › General turns automatic checks off.

## Use

| Shortcut | Does |
|---|---|
| ⌃⌥F, or right ⌥ twice | Fix the selected text in place |
| ⌃⌥T, or left ⌥ twice | Open the panel at the caret: format (Markdown, Telegram), change the tone, other actions |
| Esc | Cancel a request; the text stays as it was |

Every shortcut can be changed in Settings › Hotkeys. Russian, English and Spanish are first-class.

## Privacy

- Your text goes only to the model you chose, through your own subscription.
- The app never reads password fields, or anything while Secure Input is on. It is off in the apps you exclude (Apple Passwords by default).
- Over 10 000 characters, nothing is sent until you confirm.
- Logs hold lengths and timings, never your text. Edit history stays on this Mac, for as long as you choose, and can be turned off.
- An update check is one anonymous request for `appcast.xml` here.

## Report a problem

[Open an issue](../../issues/new/choose). Include the app version (Settings › About, click to copy) and the app you were typing in. **Don't paste private text:** describe it, or use a made-up sample.

---

Copyright © 2026 Serge Polin. All rights reserved; free to use. Third-party notices: Settings › About › Acknowledgements. Claude, ChatGPT and Grok are trademarks of their owners; Text Helper is not affiliated with or endorsed by them.
