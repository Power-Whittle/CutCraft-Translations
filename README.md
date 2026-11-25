# Cut Craft language packs

**Official, community supported.** Every pack here is checked by Cut Craft's automatic tests
and signed with Cut Craft's release key, so Cut Craft installs it as official: it holds only
words and can't run anything. The words themselves are written and kept up by volunteer
translators, not by Cut Craft's author, and nobody reads a pack by hand before it is
published. A pack that passes the checks is published.

## Install

In Cut Craft: **Gadgets ▸ Add-ons ▸ Languages**, then **Install** beside your language. Pick
it in **Edit ▸ Options ▸ Language**. Each release holds one `language-<code>.zip` per
language, and each installs on its own. Anything a pack hasn't translated yet shows in
English.

## Report a wrong or missing word

Open an [issue here](../../issues), and name the language, the words you saw and where.
The pack's translators answer here. Report anything else that goes wrong in Cut Craft from
inside Cut Craft (right-click ▸ **Report a Bug Here…**).

## New: tool names, groups, tabs and menus

Since Cut Craft PR #703, tool names, tool groups, sub-tabs, page tabs and menu items can be
translated too. Their English is in four files in Cut Craft's source:

- [tools.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/tools.ftl): every tool's name, keyed by the tool's id (`tools-draw-circle`)
- [tool-groups.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/tool-groups.ftl): group names and tool box captions (`group-create-vectors`)
- [subtabs.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/subtabs.ftl): sub-tabs with their tooltips, side tabs, browser and Ribbon tabs
- [menu-items.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/menu-items.ftl): menu bar and right-click menu items

Copy them into your pack's folder with the same names and translate the words after each `=`.
See [docs/translating.md, Tool names, groups, tabs and menus](https://github.com/NoobyNull/Cut-Craft/blob/main/docs/translating.md#tool-names-groups-tabs-and-menus).

## New: every word on screen can be translated

Since Cut Craft PRs #710 to #733, nearly every word Cut Craft shows comes from Fluent. Before,
some of it was still written into the code in English. The new words include:

- every tool's form and settings
- the tooltips and the status bar
- the hints and buttons in the windows
- Machine Configuration, the Tool Database and the Report a Bug form
- what a tool says when it cannot run

The English is in these files in Cut Craft's source:

| File | What it holds | Keys |
| --- | --- | --- |
| [settings.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/settings.ftl) | Every tool form's settings, their tooltips and choices, and the headings over them | 2,665 |
| [tooltips.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/tooltips.ftl) | What each tool does, shown in its tooltip (`tooltip-<tool id>`) | 358 |
| [status.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/status.ftl) | What the status bar says | 97 |
| [text.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/text.ftl) | Hints, headings and buttons in the windows | 361 |
| [machines.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/machines.ftl) | Machine Configuration and Post-Processor sentences with values in them | 8 |
| [tool-database.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/tool-database.ftl) | Tool Database sentences with values in them | 11 |
| [errors.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/errors.ftl) | What a tool says when it cannot run | 299 |
| [menu-items.ftl](https://github.com/NoobyNull/Cut-Craft/blob/main/crates/i18n/locales/en/menu-items.ftl) | Menu items, now also the job's right-click menus | 241 |

These join the files that could already be translated, such as `app.ftl` and `panels.ftl`.
All of Cut Craft's English is in
[crates/i18n/locales/en](https://github.com/NoobyNull/Cut-Craft/tree/main/crates/i18n/locales/en).

Copy each file into your pack's folder with the same name, then translate the words after
each `=`.

- Keys such as `setting-cut-depth-b1c2d3` are made from the English words. If the English is
  reworded, the key changes, and the new words show in English until you translate them.
- Keep each `{ $value }`, and move it to wherever your language puts it.
- In `errors.ftl`, write each message the way the English is written. Cut Craft adds the
  capital letter and the full stop itself.

For the details, see [docs/translating.md](https://github.com/NoobyNull/Cut-Craft/blob/main/docs/translating.md).
The help pages are not translatable yet; that comes later.

## Translate

The packs are made from `language-packs/` in
[Cut Craft's source](https://github.com/NoobyNull/Cut-Craft/tree/main/language-packs).
See [docs/translating.md](https://github.com/NoobyNull/Cut-Craft/blob/main/docs/translating.md)
to make or update one, and put your name in its `translators` line to be credited.
