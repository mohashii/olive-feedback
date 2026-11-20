# FAQ

## Which versions of Olive are available?

| Platform | Status |
| --- | --- |
| Mac | [Download from GitHub Releases](https://github.com/mohashii/olive-feedback/releases/latest). macOS 13.3 or later, Apple Silicon and Intel |
| Visual Studio Code | [Olive — Visual Markdown Editor on the Marketplace](https://marketplace.visualstudio.com/items?itemName=mohashi.olive-markdown). Windows, Mac and Linux |
| iPhone and iPad | In development, not released |

All of them use the same [issue tracker](https://github.com/mohashii/olive-feedback/issues).

## Is Olive open source?

No. Olive is closed source. The [olive-feedback](https://github.com/mohashii/olive-feedback) repository contains no source code; it exists so that the documentation and the issue tracker are public.

## Is it free? Will it stay free?

It is free. For the VS Code extension, if a future version is offered for a fee, versions that were distributed free of charge remain usable free of charge — see [LICENSE-extensions](https://github.com/mohashii/olive-feedback/blob/main/LICENSE-extensions) §2.

## Does Olive change my Markdown files?

Only where you edit. Constructs Olive cannot edit as rich text are kept verbatim — raw HTML blocks, for example, are shown as a preserved block with their source — so nothing is silently dropped or rewritten. A file you open and save without editing is byte-identical to what it was.

A few actions reach beyond the note in front of you, and each follows from something you did:

- Renaming or moving a note rewrites the links that point at it in other notes, and Olive tells you how many. See [Links follow renames](links.md#links-follow-renames).
- Pasting or dropping an image saves it to an `assets/` folder beside the note.

**In the Mac app:** when you delete an image from a note and no other note uses it, Olive removes the file from `assets/` the next time the note is saved. See [Images](images.md#images-when-notes-move).

## Does Olive take over `.md` files?

No.

- **In the Mac app:** Olive offers to open `.md` files — it appears in Finder's **Open With** menu — but it does not make itself the default app, so double-clicking one in Finder still opens whatever app you had before until you choose otherwise. See [Opening a single file](mac.md#opening-a-single-file).
- **In VS Code:** VS Code's text editor stays the default, and you open a file in Olive yourself — through the Olive icon on the editor title bar, **Open in Olive** in the Explorer, or **Reopen Editor With…**. You can make Olive the default with `workbench.editorAssociations`; see [Olive for Visual Studio Code](vscode.md).

## Does Olive send anything anywhere?

No telemetry and no analytics, and Olive never sends your notes anywhere. The few cases in which it goes online at all — including the Mac app's check for updates — are listed under "Network access" in the [privacy policy](https://github.com/mohashii/olive-feedback/blob/main/PRIVACY.md#network-access).

## How does the Mac app update?

It keeps itself up to date: a new version is downloaded quietly and used the next time you open Olive, without interrupting you to restart. **Olive ▸ Check for Updates…** checks straight away. When the app checks, and what that request contains, is described in the [privacy policy](https://github.com/mohashii/olive-feedback/blob/main/PRIVACY.md#network-access).

## Which Markdown dialect does Olive use?

CommonMark plus GitHub Flavored Markdown (tables, task lists, strikethrough, footnotes), with `$…$` and `$$…$$` for math. Callouts use the blockquote-with-marker form (`> [!note]`), as GitHub alerts and Obsidian callouts do, and Obsidian-style `[[wikilinks]]` are recognised. Anything Olive does not recognise is kept exactly as written. The details are in [Markdown compatibility](markdown-compatibility.md).

## How is the VS Code extension different from VS Code's built-in Markdown editor?

Both let you edit rendered Markdown. Olive is aimed at technical documents: TeX math rendered with KaTeX and re-editable in its own input, tables you work with as structure, callouts, toggles and Mermaid diagrams that stay editable, and Markdown markers that stay hidden even inside the element the cursor is in. The two can coexist — installing Olive does not affect the built-in editor.

## Does the VS Code extension work over SSH, WSL, Dev Containers or Codespaces?

Untested in this release. It may work, but nothing has been verified. Untrusted workspaces and virtual workspaces are not supported, and Olive stays disabled in them.

## Where is the changelog?

- **Mac:** the release notes on [GitHub Releases](https://github.com/mohashii/olive-feedback/releases).
- **VS Code:** the extension's [Marketplace Changelog tab](https://marketplace.visualstudio.com/items?itemName=mohashi.olive-markdown&ssr=false#version-history).

---

Back to the [contents](README.md).
