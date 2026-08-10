# Troubleshooting

Things that turn out to have a local cause. If none of these apply, please
[open a bug report](https://github.com/mohashii/olive-feedback/issues/new?template=bug_report.yml).

## Olive is missing from "Reopen Editor With…"

Olive declares itself unsupported in two situations and VS Code hides it accordingly:

- **Restricted Mode (untrusted workspace).** The banner at the top of the window tells
  you when a folder is not trusted. Olive stays disabled until you trust the folder.
- **Virtual workspaces** (a remote file system with no local files, e.g. the GitHub
  Repositories extension). Not supported in this release.

## I trusted the folder, but the file still opens as plain text

**Close the editor tab and open the file again.** Reopening the file while the tab is
still open reuses the existing text editor, so nothing appears to change. This also
applies right after you install the extension or change
`workbench.editorAssociations`.

## `workbench.editorAssociations` has no effect

The viewType is `olive.markdown`:

```json
"workbench.editorAssociations": {
  "*.md": "olive.markdown"
}
```

A workspace-level setting overrides your user setting — check both. Olive never sets
this for you; it stays an opt-in.

## A keyboard shortcut does nothing, or does the wrong thing

Olive's editing commands are ordinary VS Code commands and appear under **Olive** in the
Keyboard Shortcuts editor (`⌘K ⌘S` / `Ctrl+K Ctrl+S`). Search for the action there — the
editor shows when another extension or a user binding has claimed the same keys, and you
can rebind either side.

A few keys belong to the editing surface rather than to a command and cannot be rebound:
`Shift+Enter` for a hard line break, `⌘⇧↑` / `⌘⇧↓` to move blocks, and `Option/Alt` with
the arrow keys to move table rows and columns.

## Part of my document shows as a source block instead of rich text

That is deliberate: Olive keeps constructs it cannot edit as rich text verbatim, and
shows them explicitly rather than hiding or rewriting them. The file round-trips
unchanged.

If it is a construct you would expect Olive to handle, that is worth a report — please
include the smallest snippet that produces the block.

## Unsaved changes appeared to come back after "Don't Save"

When a file is open in more than one editor and you discard changes in one of them,
Olive keeps the unsaved content in the view that is still open, without a notification.
Closing the last view discards as normal, and **File: Revert File** always reverts.

If your content came back when you expected it gone, or vanished when you expected it
kept, please report it with the exact sequence of tabs and clicks — this area is timing
sensitive and the sequence is the useful part.

## It behaves differently over SSH / WSL / Dev Containers / Codespaces

These are untested in this release. Reports are welcome, but please say which one you
are using — it is the first thing that will be asked.
