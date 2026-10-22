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

Raw HTML blocks, and anything else Olive cannot edit as rich text, are shown as a preserved block: a sanitized rendering of what the Markdown means, with a small **Kept as written** label. Click **Edit** on that label, or use **Edit Markdown** from the [block menu](blocks.md#the-block-menu), to change the source in place. You can see both how the block will look and exactly what Olive is not editing for you.

Inline HTML inside a paragraph is edited as ordinary text instead. Paired tags such as `<b>x</b>` are shown formatted, `<a href>` works as a link, and empty tags such as `<br>` and `<img>` are shown as single objects you can select and delete. Whatever Olive cannot present is left as literal text, and the original spelling is written back unchanged.

A few constructs Olive has no model for, such as `:::note` container directives and definition lists, appear as ordinary paragraphs. They are kept exactly as written.

**In the Mac app:** if a block cannot be written back safely, Olive stops saving that note automatically and says "1 block cannot be saved" next to the note's save status, so nothing is overwritten without you knowing; see [Saving and recovery](saving-and-recovery.md#blocks-olive-cannot-write-back).

---

Back to the [contents](README.md).
