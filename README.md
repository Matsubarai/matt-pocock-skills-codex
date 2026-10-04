# Matt Pocock Skills for Codex

Unofficial, minimal Codex packaging of the **27 official skills** from [mattpocock/skills](https://github.com/mattpocock/skills), pinned to commit [`d81f3a183412e71a5b1e84ca21bc1a35eea03a60`](https://github.com/mattpocock/skills/tree/d81f3a183412e71a5b1e84ca21bc1a35eea03a60).

Version: **0.1.9**. This project excludes upstream `in-progress` and miscellaneous skills.

## Plugin

[Matt Pocock Skills Original](https://chatgpt.com/plugins/plugins_6ac2a64bb6f8819193239b535e37188f) is the existing private plugin; access depends on the account that created it. This repository contains its source. Publishing this repository does not publish the plugin to the public plugin directory.

The portable manifest is [plugin.json](plugin.json). The Codex compatibility manifest is [.codex-plugin/plugin.json](.codex-plugin/plugin.json). All 27 skills are declared there. The local marketplace manifest is [.agents/plugins/marketplace.json](.agents/plugins/marketplace.json).

## Minimal adaptations

- Preserve skill names, workflows, scripts, dependencies, and invocation policies.
- Remove `CLAUDE.md` references from the affected skill instructions, retaining the existing `AGENTS.md` selection rules.
- Change only the two `Mechanics:` configuration clauses in `writing-for-agents/SKILL-MECHANICS.md` to Codex policy fields.
- Place skills at `skills/<name>/` for account plugin discovery. Preserve each skill's internal files byte for byte relative to the prepared Codex version.
- Update only 62 relative links in the upstream README and the two category indexes for this directory relocation. Keep `docs/` byte-identical to upstream.

See [PROVENANCE.json](PROVENANCE.json) for original Git blob hashes, current SHA-256 hashes, source paths, adaptations, and directory relocations. [CONTENT-DIFF.patch](audit/CONTENT-DIFF.patch) records textual differences against the pinned upstream commit; [DIRECTORY-MAP.json](audit/DIRECTORY-MAP.json) separately records directory moves. [UPLOAD-LINK-CHANGES.patch](audit/UPLOAD-LINK-CHANGES.patch) records the upload-specific link edits.

[UPSTREAM-README.md](UPSTREAM-README.md) and [UPSTREAM-CHANGELOG.md](UPSTREAM-CHANGELOG.md) retain upstream documentation. Some documents describe Claude Code behavior; they are preserved historical documentation, not a guarantee of identical Codex runtime behavior.

## License and attribution

Original skills by **Matt Pocock and contributors**, under the [MIT license](LICENSE). This repository is an unofficial adaptation, not endorsed by the upstream authors.
