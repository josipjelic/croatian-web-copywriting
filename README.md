# croatian-web-copywriting

Plugin for Claude, ChatGPT and Codex with one skill: writes and edits short-form website copy in natural,
native-sounding Croatian — hero headlines, CTAs, buttons, form microcopy, 404 pages,
meta titles and descriptions — so it doesn't read as translated from English.

Made by [Kontekst](https://kontekst.hr).

## Install (Claude Code)

```
/plugin marketplace add josipjelic/croatian-web-copywriting
/plugin install croatian-web-copywriting@kontekst
```

The skill triggers on its own when you write or review Croatian web copy.

## Install (Codex CLI)

```
codex plugin marketplace add josipjelic/croatian-web-copywriting
codex plugin add croatian-web-copywriting@kontekst
```

## Install (ChatGPT)

1. In the ChatGPT desktop app, turn on Settings → Security and login → Developer mode.
2. Register the marketplace with `codex plugin marketplace add josipjelic/croatian-web-copywriting`
   (the desktop app reads the same sources), then restart the app.
3. Open Plugins, pick the **Kontekst** marketplace and install **Croatian Web Copywriting**.

Once installed it works in ChatGPT on web, desktop and mobile. You can also call it
explicitly with `@` in a new conversation.

## Layout

- `skills/croatian-web-copywriting/` — the skill itself (shared by every host)
- `plugin.json` — portable Agent Plugins manifest read by ChatGPT and Codex
- `.agents/plugins/marketplace.json` — ChatGPT/Codex marketplace
- `.claude-plugin/` — Claude Code plugin and marketplace manifests

When you bump the version, update both `plugin.json` and `.claude-plugin/plugin.json`.

## Contributing

Contributions are welcome — especially from native Croatian speakers who spot copy
that still sounds translated.

- **Report a problem:** open an issue with the prompt you used, the copy you got, and
  what a Croatian writer would have said instead.
- **Improve the guidance:** the rules live in `skills/croatian-web-copywriting/SKILL.md`
  and its `references/` files. Keep examples short and concrete, show a bad line next to
  its fix, and keep the existing tone and structure of each file.
- **Add test cases:** `skills/croatian-web-copywriting/evals/evals.json` holds prompts
  used to check the skill. Add one for any behaviour you fix, so it doesn't regress.
- **Pull requests:** keep each PR focused on one change and describe what it fixes.
  If you change the plugin itself (not just the skill), bump the version in both
  `plugin.json` and `.claude-plugin/plugin.json`.

For questions or collaboration, get in touch through [kontekst.hr](https://kontekst.hr).
