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

## Translate

The packs are made from `language-packs/` in
[Cut Craft's source](https://github.com/NoobyNull/Cut-Craft/tree/main/language-packs).
See [docs/translating.md](https://github.com/NoobyNull/Cut-Craft/blob/main/docs/translating.md)
to make or update one, and put your name in its `translators` line to be credited.
