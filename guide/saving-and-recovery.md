# Saving and recovery

This page is about the Mac app. In VS Code, saving and file history are VS Code's own.

## How Olive saves

Olive saves a note by itself about two seconds after you stop typing, and keeps a draft of your edits on this Mac even sooner, so nothing is lost if the app quits before the file is written. `⌘S`, or **Save now** in the note's **…** menu, saves straight away. To save only when you ask, uncheck **Auto-save** in the same menu.

While Olive saves by itself, the note's header says nothing about saving. It shows one of these only when you need to act:

| Shown | Meaning |
| --- | --- |
| ● Unsaved | Auto-save is off and you have edits that are not written yet. `⌘S` writes them |
| ● Draft saved | Auto-save is off and your edits are kept on this Mac, but not yet written to the file. `⌘S` writes them |
| ● Auto-save failed | Olive could not write the file. Your edits are kept on this Mac; `⌘S` tries again |
| ● Draft save failed | Olive could not keep a draft of your edits on this Mac |
| ● 1 block cannot be saved | See [Blocks Olive cannot write back](#blocks-olive-cannot-write-back) |
| ⚠ Changed externally — Resolve | See [When a file changes outside Olive](#when-a-file-changes-outside-olive) |

If Olive quits with unsaved edits, they come back the next time you open the note.

## When a file changes outside Olive

Another editor, a sync service or Git may change a note while it is open.

- **If you have no unsaved edits,** Olive simply shows the new version.
- **If you do,** Olive combines both sets of changes and says how many outside changes it merged. **Undo** on that message takes the merge back.
- **If the two cannot be combined,** the header shows **Changed externally — Resolve** and Olive stops saving that note automatically. Click it, or press `⌘S`, to open a window that shows each conflict and lets you keep your version, take the other one, or keep both, before **Save resolved**.

The same window appears when iCloud Drive leaves two versions of a note, such as `Note 2.md` beside `Note.md`.

## Notes in iCloud Drive

Notes that iCloud Drive has not downloaded to this Mac are downloaded when you open them. If one cannot be downloaded — while offline, for example — Olive shows the last copy it read, marked read-only.

## File recovery

Olive keeps a copy of each note before it is overwritten: the last five versions, on this Mac only. Choose **File recovery…** from the note's **…** menu to see them, with the differences from what you have now. **Recover this version** puts that version in the editor, and it is saved like any other edit — within a couple of seconds while Auto-save is on.

Versions taken before an outside change was merged, or from a conflicting copy, are labelled as such.

## Blocks Olive cannot write back

Very rarely, Olive cannot write a block back exactly as it was written. It then stops saving that note automatically, so nothing changes without you knowing, and the header shows **1 block cannot be saved**. Press `⌘S` to see the block as it is now and as it would be saved, and choose **Save changed version** or **Cancel**. **Copy details** copies a description you can attach to a [bug report](https://github.com/mohashii/olive-feedback/issues/new?template=bug_report.yml).

---

Back to the [contents](README.md).
