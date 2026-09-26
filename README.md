# croatian-web-copywriting

Plugin for Claude, ChatGPT, Codex and Cursor with one skill: writes and edits short-form website copy in natural,
native-sounding Croatian — hero headlines, CTAs, buttons, form microcopy, 404 pages,
meta titles and descriptions — so it doesn't read as translated from English.

Made by [Kontekst](https://kontekst.hr).

## Install (Claude Code)

```
/plugin marketplace add josipjelic/croatian-web-copywriting
/plugin install croatian-web-copywriting@kontekst
```

The skill triggers on its own when you write or review Croatian web copy.

**Auto-update.** Auto-update is off by default for third-party marketplaces. Turn it on
in `/plugin` → **Marketplaces** → **kontekst** → enable auto-update, or update by hand
with `/plugin marketplace update kontekst`. Claude Code only sees a new release when the
`version` in the manifests goes up.

**Per project (and Claude Code on the web).** To enable the plugin for everyone working
in a repo, including cloud sessions on claude.ai/code, commit this as
`.claude/settings.json` in that repo:

```json
{
  "extraKnownMarketplaces": {
    "kontekst": {
      "source": { "source": "github", "repo": "josipjelic/croatian-web-copywriting" }
    }
  },
  "enabledPlugins": {
    "croatian-web-copywriting@kontekst": true
  }
}
```

Each cloud session installs the plugin fresh from `main`, so it always runs the latest
version. If the repo already has a `.claude/settings.json`, merge these two keys into it.

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

## Install (Cursor)

Once the plugin is listed in the [Cursor Marketplace](https://cursor.com/marketplace):
open **Customize** in the sidebar, find **Croatian Web Copywriting** and select
**Install** (project or user scope). Call it explicitly with `/croatian-web-copywriting`
in chat, or let it trigger on its own.

To use it before then, clone the repo into `~/.cursor/plugins/local/croatian-web-copywriting`
and run **Developer: Reload Window**. Teams can also add it through
Dashboard → Plugins & MCPs → Team Marketplaces → Import from Repo.

## Layout

- `skills/croatian-web-copywriting/` — the skill itself (shared by every host)
- `plugin.json` — portable Agent Plugins manifest read by ChatGPT and Codex
- `.agents/plugins/marketplace.json` — ChatGPT/Codex marketplace
- `.claude-plugin/` — Claude Code plugin and marketplace manifests
- `.cursor-plugin/plugin.json` — Cursor plugin manifest

When you bump the version, update `plugin.json`, `.claude-plugin/plugin.json` and
`.cursor-plugin/plugin.json`.

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
  Bump the version in all three manifests (`plugin.json`, `.claude-plugin/plugin.json`,
  `.cursor-plugin/plugin.json`) for any change, skill text included, so installed
  copies pick it up.

For questions or collaboration, get in touch through [kontekst.hr](https://kontekst.hr).
