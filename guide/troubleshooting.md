# Troubleshooting

Things that turn out to have a local cause. If none of these apply, please [open a bug report](https://github.com/mohashii/olive-feedback/issues/new?template=bug_report.yml).

## Part of my document shows as a source block instead of rich text

That is deliberate: Olive keeps constructs it cannot edit as rich text exactly as written, and shows them openly rather than hiding or rewriting them. The file round-trips unchanged.

If it is a construct you would expect Olive to handle, that is worth a report — please include the smallest snippet that produces the block.

## In the Mac app

### Olive will not open on my Mac

Olive for Mac needs macOS 13.3 or later. It runs on both Apple Silicon and Intel Macs.

### Olive opened a folder I did not expect

The first time Olive starts on a Mac with iCloud Drive, it creates a folder named **Olive** in iCloud Drive and opens it; if a folder with that name is already there, it opens that one. After that, Olive opens the last folder you used. To work in another folder, click the ⌃⌄ beside the folder name at the bottom of the sidebar and choose **Open another folder…**, or choose **File ▸ Open Folder…**. See [Olive for Mac](mac.md#your-first-folder).

### A note opens read-only

The note is in iCloud Drive but not downloaded to this Mac, and it could not be downloaded — usually because the Mac is offline. Olive shows the last copy it read, marked read-only, so that an old version is never written back. Open the note again once you are online. See [Notes in iCloud Drive](saving-and-recovery.md#notes-in-icloud-drive).

### The note's header says "Changed externally — Resolve"

Another app, a sync service or Git changed the note while you had edits that Olive could not combine with them. Olive stops saving that note on its own until you choose what to keep. Click the message, or press `⌘S`. See [When a file changes outside Olive](saving-and-recovery.md#when-a-file-changes-outside-olive).

### The note's header says "1 block cannot be saved"

See [Blocks Olive cannot write back](saving-and-recovery.md#blocks-olive-cannot-write-back). **Copy details** there copies a description you can attach to a bug report.

### "Check for Updates…" says it could not check

Olive could not reach GitHub, where it looks for new versions — usually because the Mac is offline. Try again later. You can always download the latest version from [GitHub Releases](https://github.com/mohashii/olive-feedback/releases/latest) and replace the app in **Applications**; your notes are not inside the app, so nothing is lost.

## In VS Code

### Olive is missing from "Reopen Editor With…"

Olive declares itself unsupported in two situations, and VS Code hides it accordingly:

- **Restricted Mode (untrusted workspace).** The banner at the top of the window tells you when a folder is not trusted. Olive stays disabled until you trust the folder.
- **Virtual workspaces** (a remote file system with no local files, such as the GitHub Repositories extension). Not supported in this release.

### I trusted the folder, but the file still opens as plain text

**Close the editor tab and open the file again.** Reopening the file while the tab is still open reuses the existing text editor, so nothing appears to change. This also applies right after you install the extension or change `workbench.editorAssociations`.

### `workbench.editorAssociations` has no effect

The viewType is `olive.markdown`:

```json
"workbench.editorAssociations": {
  "*.md": "olive.markdown"
}
```

A workspace-level setting overrides your user setting — check both. Olive never sets this for you; it stays an opt-in.

### A keyboard shortcut does nothing, or does the wrong thing

Olive's editing commands are ordinary VS Code commands and appear under **Olive** in the Keyboard Shortcuts editor (`⌘K ⌘S` / `Ctrl+K Ctrl+S`). Search for the action there — the editor shows when another extension or a user binding has claimed the same keys, and you can rebind either side.

Moving blocks (`⌥↑` / `⌥↓`, `Alt+↑` / `Alt+↓` on Windows and Linux) and opening block actions (`⌘/` / `Ctrl+/`) and **Edit Markdown** (`⌥⌘U` / `Ctrl+Alt+U`) are commands too, so they can be rebound there. `Shift+Enter` for a hard line break belongs to the editing surface rather than to a command and cannot be rebound. Table rows and columns have no keyboard shortcut; move them from the table's right-click menu or the slash menu.

### Unsaved changes appeared to come back after "Don't Save"

When a file is open in more than one editor and you discard changes in one of them, Olive keeps the unsaved content in the view that is still open, without a notification. Closing the last view discards as normal, and **File: Revert File** always reverts.

If your content came back when you expected it gone, or vanished when you expected it kept, please report it with the exact sequence of tabs and clicks — this area is timing sensitive and the sequence is the useful part.

### It behaves differently over SSH, WSL, Dev Containers or Codespaces

These are untested in this release. Reports are welcome, but please say which one you are using — it is the first thing that will be asked.

---

Back to the [contents](README.md).
