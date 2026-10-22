# Links and footnotes

## Links

Select text and press `⌘K` (`Ctrl+K`), or use the link button on the selection toolbar. With nothing selected, `⌘K` inserts a new link. The link form has the **URL** and the **Label**, and **Apply**; for a link that already exists it also offers **Open** and **Remove**. Pointing at a link shows where it goes.

Clicking a link:

- a link to another `.md` file in the folder opens that note in Olive
- a `#heading` link jumps to that heading in the same note
- anything else opens in your web browser; a link that would hand off to another app asks first

**In the Mac app:** a link to another kind of file in the folder — a PDF, a picture — opens a preview inside Olive.

## Page links

Type `[[` to search the Markdown files in your folder and link one. Olive writes an ordinary Markdown link, `[name](relative/path.md)`, so the note stays readable in any other editor.

Obsidian-style wikilinks work too: `[[name]]`, `[[name|label]]`, `[[name#heading]]`, and `[[#heading]]` for a heading in the note you are in. Clicking one opens it. If you write a wikilink out by hand and close the `]]`, it becomes a wikilink there and then, so you can keep writing them if that is your habit — the `[[` search above is simply the way Olive inserts links itself.

A wikilink is treated as one word. The caret sits before or after it rather than inside, the arrow keys step over it, and one `Backspace` removes the whole thing. Its spelling is written back exactly as it stands, and editing the text around it leaves it alone. To change it, right-click it or press `⌘K` to edit its label or target, which keeps the `[[…]]` form; **To Markdown link** in that form turns it into an ordinary link.

## Links follow renames

When you rename or move a note — in the sidebar of the Mac app, or in VS Code's Explorer — Olive rewrites the links that pointed at it, and the links inside it that pointed elsewhere. This covers ordinary Markdown links and wikilinks alike.

- Inside a `[[…]]`, only the note name is rewritten; an alias after `|` and a `#heading` are left alone.
- A Markdown link whose text is just the old file name is relabelled with the new one.
- When notes other than the one you renamed had to change, Olive tells you how many.

**In the Mac app:** the message reads "Updated links in 2 other notes" and has an **Undo** button. If some notes could not be updated, the message says so and stays until you close it.

## Footnotes

A footnote reference such as `[^1]` stays compact in the sentence, and its definition, `[^1]: …`, appears as a quieter block that you edit like any other text.

- **To add one,** type `[^label]` in the sentence and keep typing; the reference forms on the next character. If that label has no definition yet, Olive adds an empty one at the end of the note. To write a definition yourself, type `[^label]: ` at the start of a line.
- **Click a reference** to jump to its definition. **Click the label** of a definition to go back to the reference you came from.
- **Right-click** a reference or a definition's label to open a card with the footnote, without jumping.

Labels cannot contain spaces or tabs. That is a GitHub Markdown rule rather than an Olive one, so `[^my note]` stays plain text.

---

Back to the [contents](README.md).
