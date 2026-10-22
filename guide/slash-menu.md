# The slash menu

Type `/` to change the block you are in or to insert a new one. Keep typing to filter the list, use the arrow keys to move, and press `Enter` to run the highlighted command. `Esc` closes the menu.

Each command always does the same thing, and the menu groups them by what they do:

- **Turn into** — converts the block you are typing in and keeps its text. On an empty line this simply creates the block; inside a list it converts just the item you are on.
- **Insert** — always adds a new block. An empty line is used as the spot to insert; from a line with content, the new block lands right below it.
- **Callout** — shown only inside a callout. **Edit callout…** opens the callout's title, type and fold settings; **Add title** or **Remove title** appears, whichever applies.

Inside a table the menu offers table commands instead; see [Tables](tables-callouts-diagrams.md#tables).

## Commands

| Block | Search for |
| --- | --- |
| Text (paragraph) | `/text`, `/paragraph`, `/plain` |
| Heading 1–5 | `/h1` – `/h5`; also `/title`, `/section`, `/subsection`, `/subsubsection` for heading 1–4 |
| Bulleted list | `/bullet`, `/list` |
| Numbered list | `/numbered` |
| Task list | `/todo` |
| Quote | `/quote` |
| Code block | `/code` |
| Mermaid diagram | `/mermaid`, `/diagram`, `/flowchart`, `/chart`, `/graph` |
| Math block | `/math`, `/equation`, `/tex`, `/latex` |
| Callout | `/callout`, `/note` |
| Toggle | `/toggle` |
| Table | `/table` |
| Image | `/image`, `/picture`, `/photo`, `/figure` |
| Divider | `/divider`, `/hr`, `/rule`, `/separator` |
| HTML | `/html`, `/raw`, `/embed`, `/iframe`, `/markup` |

Search ignores case and matches the block names as well as the words above, with closer matches listed first. Typing a character other than a letter, digit, space or hyphen dismisses the menu.

**HTML** inserts an empty raw HTML block and opens its source for editing. Olive shows a sanitized rendering of it; see [Markdown compatibility](markdown-compatibility.md#blocks-olive-keeps-as-written).

## Turning an existing block into something else

The same **Turn into** list is on the block's handle menu, which also works on a selection of several blocks. See [Blocks](blocks.md).

---

Back to the [contents](README.md).
