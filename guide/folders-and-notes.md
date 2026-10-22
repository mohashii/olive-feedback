# Folders and notes

This page is about the Mac app. In VS Code, files are managed by VS Code's own Explorer.

## Notes and folder pages

Click a note in the sidebar to open it. Click a folder to open its **folder page**, which shows cards for everything inside it. To expand or collapse a folder in the sidebar without opening it, click the arrow at the right end of its row.

A folder can have a **folder note**: a note named `index.md` inside it, shown at the top of the folder page above the cards. Choose **Add folder note** from the folder's right-click menu, or from the **…** menu on its page. The folder note of the top folder is your home page. `index.md` files are not listed separately in the sidebar.

## Creating notes and folders

- **New note** at the bottom of the sidebar creates a note in the top folder.
- **New note** and **New folder** are in a folder's right-click menu, in the **+** that appears when you point at a folder, and in the **+** at the bottom of a folder page.

A new note is named `Untitled` with today's date until you give it a title. Type the title at the top of the note; Olive renames the file to match when it saves.

### The title and the file name

While **File name follows title** is checked in the note's **…** menu, saving renames the file to match the title. Characters that file names cannot hold, such as `/` and `:`, become `-`. If another file already has that name, Olive tells you, keeps the file name as it is and puts the title back to match it (a new `Untitled` note gets an empty title again). Uncheck it to keep the file name as it is whatever the title says.

## Renaming, moving and deleting

Right-click a note or folder for its actions:

| Item | Notes |
| --- | --- |
| Open in new window | |
| Rename | Or select the row and press `Enter`. `Esc` cancels |
| Duplicate | Notes only. The copy is named `Name (1)` |
| Export as HTML… | Folders only; see [Export](export.md) |
| Delete file / Delete folder | Moves it to the Trash |

If a note's front matter has an `icon:` — for instance because it came from Notion — that icon is shown beside the name. This release has no way to set one.

To move notes and folders, drag them onto another folder. `⌘`-click or `Shift`-click to drag several at once. While the sidebar has focus, `⌘Z` undoes a move or rename.

Renaming or moving a note also updates the links to it; see [Links follow renames](links.md#links-follow-renames).

### Recently Deleted

Deleted notes and folders go to the macOS Trash, and Olive also keeps a copy for 30 days. Choose **Recently Deleted…** from the **…** menu at the top of the sidebar to bring one back with **Restore**. Restoring never replaces a file that is there now; if the name is taken, the restored note is called `Name (restored)`.

The same window lists notes under **Missing from the folder** when Olive still has a copy but the file is no longer there — deleted or moved outside Olive, or still syncing.

## Other files

With **Show other files** on (in Settings), files that are not Markdown appear in the sidebar too. Pictures and PDFs open in a preview inside Olive; for other kinds, Olive offers **Open in default app**, **Reveal in Finder** and **Save a copy…**. The `assets` folders that hold your notes' images are never listed.

## Favorites

To return quickly to a folder you use often, open it with **Open another folder…** and choose **Add to favorites** from the **…** menu at the top of the sidebar. The folder Olive opened first is already there. Your favorite folders are listed in that menu from then on.

## Daily notes

Click the calendar at the bottom of the sidebar, or press `⌥⌘N`, to open today's note. It is created if it does not exist yet, at `Daily/2026/10/2026-10-06.md` for 6 October 2026.

Daily notes are on whenever the folder has a top-level folder named `Daily`. Olive creates one in the folder it sets up for you on first launch. To turn daily notes on or off elsewhere, use **Daily notes** in Settings; turning them off moves the `Daily` folder and its notes to the Trash, from where **Recently Deleted** can bring them back.

## Getting around

- **Back** and **Forward** — `⌘[` and `⌘]`, the arrows beside the window buttons, or a two-finger swipe on the trackpad.
- **Go to the parent folder** — the up arrow beside them.
- **Home** — click the folder name at the top of the sidebar.

## Search

Click the magnifier at the bottom of the sidebar, or press `⇧⌘F`, and type. Olive searches file names and the text of every note, and lists each matching note with up to five matching lines. Click a line to open the note at that place, or the note's name to open it from the top. `Enter` opens the first match. **Aa** makes the search match case, and `Esc` clears the search, then closes it.

Notes stored in iCloud Drive that are not downloaded to this Mac are downloaded to be searched, and the result says how many.

To search within the open note instead, press `⌘F`.

## Outline

The headings of the open note are listed under it in the sidebar. Click a heading to jump to it, or drag it to move the whole section. Right-click a heading to **Promote** or **Demote** it, **Select section**, or choose how many levels to show. The arrow on the note's row hides or shows the outline.

---

Back to the [contents](README.md).
