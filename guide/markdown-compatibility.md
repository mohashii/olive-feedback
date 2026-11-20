# Markdown compatibility

Olive edits plain Markdown files and writes plain Markdown back. Nothing is stored anywhere except the `.md` file and the images beside it.

## The Markdown Olive understands

- **CommonMark** with the **GitHub Flavored Markdown** additions: tables, task lists, strikethrough, footnotes.
- **Math** as `$…$` and `$$…$$`, and GitHub's `` $`…`$ `` for an inline formula that contains a `$`.
- **Callouts** in the quote-with-marker form, `> [!note]`, as GitHub alerts and Obsidian callouts use.
- **Highlight** as `==text==`.
- **Wikilinks** as `[[note]]`, `[[note|label]]`, `[[note#heading]]` and `[[#heading]]` — read wherever they appear, written back exactly as they stand, and formed as you type if you write one out. The `[[` search inserts an ordinary Markdown link instead.
- **Toggles** as HTML `<details>` blocks with a `<summary>`.
- **Front matter** — YAML between `---` lines at the top of a file — kept exactly as written and not shown as text on the page.

## Your file comes back unchanged

Olive keeps your original text for everything you did not edit. Opening a file and saving it without changes gives back a byte-for-byte identical file, and the parts you never touched are never re-wrapped or tidied up.

## Blocks Olive keeps as written

Raw HTML blocks, and anything else Olive cannot edit as rich text, are shown as a preserved block: a sanitized rendering of what the Markdown means, with no buttons or label on it. Click or tap the block to edit its source in place, with a live preview; clicking a link in the block opens the link instead. If Olive cannot render the block faithfully — a fragment of a table, a `</div>` on its own, an HTML comment — it shows the source itself in a dotted frame labelled **Kept as written**.

Inline HTML inside a paragraph is edited as ordinary text instead. Paired tags such as `<b>x</b>` are shown formatted, `<a href>` works as a link, `<br>` is an ordinary line break, and other empty tags such as `<img>` are shown as single objects you can select and delete. Whatever Olive cannot present is left as literal text, and the original spelling is written back unchanged.

A few constructs Olive has no model for, such as `:::note` container directives and definition lists, appear as ordinary paragraphs. They are kept exactly as written.

**In the Mac app:** if a block cannot be written back safely, Olive stops saving that note automatically and says "1 block cannot be saved" next to the note's save status, so nothing is overwritten without you knowing; see [Saving and recovery](saving-and-recovery.md#blocks-olive-cannot-write-back).

## Line breaks

A line break made with `Shift+Enter` is written in whichever standard form fits where it stands:

| Where the line break is | Written as |
|---|---|
| In the middle of a paragraph, list item or quote | `\` at the end of the line |
| At the end of a paragraph, list item or quote | `<br>` |
| In a heading or a table cell | `<br>` |

The end of a paragraph needs `<br>` because a trailing `\` is read as a literal backslash when nothing follows it. Line breaks already in your file — `\`, two trailing spaces or `<br>` — keep their spelling, even in a paragraph you edit. A paragraph that holds nothing but one line break is written as `<p><br></p>`, the HTML for that paragraph, since Markdown has no way to write it; Olive reads it back as the same paragraph. With two or more line breaks, the paragraph starts with `\` and ends with `<br>`.

---

Back to the [contents](README.md).
