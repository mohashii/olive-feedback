# Folders and notes

This page is about the Mac app. In VS Code, files are managed by VS Code's own Explorer.

## Notes and folder pages

Click a note in the sidebar to open it. Click a folder to expand or collapse it; `⌥`-click to do the same to every folder inside it. To open a folder's **folder page**, which shows cards for everything inside it, click the ↗ that appears at the right end of its row when you point at it, choose **Open folder page** from its right-click menu, or select the row and press `Enter`.

A folder can have a **folder note**: a note named `index.md` inside it, shown at the top of the folder page above the cards. Open the folder's page and choose **Add folder note** from its **…** menu. The folder note of the top folder is your home page. `index.md` files are not listed separately in the sidebar.

## Creating notes and folders

- **New note** (the pencil at the top of the sidebar, or **File ▸ New Note**, `⌘N`) creates a note.
- **New note** and **New folder** are in a folder's right-click menu, in the **+** that appears when you point at a folder or at the folder name at the bottom of the sidebar, and in the **+** at the bottom of a folder page.
- In **Go to Note** (`⌘P`), type a name that no note has and choose **Create** to make a note with that name.

A new note is named `Untitled` with today's date until you give it a title. Type the title at the top of the note; Olive renames the file to match when it saves.

### The title and the file name

While **File name follows title** is checked in the note's **…** menu, saving renames the file to match the title. Characters that file names cannot hold, such as `/` and `:`, become `-`. If another file already has that name, Olive tells you, keeps the file name as it is and puts the title back to match it (a new `Untitled` note gets an empty title again). Uncheck it to keep the file name as it is whatever the title says.

## Renaming, moving and deleting

Right-click a note or folder for its actions:

| Item | Notes |
| --- | --- |
| Open folder page | Folders only |
| Open in new window | |
| Reveal in Finder | |
| Export as HTML… | Folders only; see [Export](export.md) |
| Rename | Or select the row and press `F2`. `Esc` cancels |
| Change icon… | Gives the note or folder an emoji icon |
| Duplicate | Notes only. The copy is named `Name (1)` |
| Delete file / Delete folder | Moves it to the Trash. Or select the row and press `⌘⌫` |

The icon is stored as `icon:` in the note's front matter (for a folder, in its `index.md`), so notes that came from Notion with an icon show it too. **Change icon…** is also in the note's **…** menu and in **File**.

To move notes and folders, drag them onto another folder. `⌘`-click or `Shift`-click to drag several at once. While the sidebar has focus, `⌘Z` undoes a move or rename.

Renaming or moving a note also updates the links to it; see [Links follow renames](links.md#links-follow-renames).

### Recently Deleted

Deleted notes and folders go to the macOS Trash, and Olive also keeps a copy for 30 days. Choose **Recently Deleted…** from the menu on the folder name at the bottom of the sidebar (or **Go ▸ Recently Deleted**) to bring one back with **Restore**. Restoring never replaces a file that is there now; if the name is taken, the restored note is called `Name (restored)`.

Recently Deleted lists only what you deleted in Olive. To bring back a note deleted outside Olive — in Finder, on another device, or by a sync service — use the Trash, iCloud Drive's Recently Deleted, or the version history of the service that holds the folder.

## Other files

With **Show other files** on (in Settings), files that are not Markdown appear in the sidebar too. Pictures and PDFs open in a preview inside Olive; for other kinds, Olive offers **Open in default app**, **Reveal in Finder** and **Save a copy…**. The `assets` folders that hold your notes' images are never listed.

## Favorites

To return quickly to a folder you use often, open it with **Open another folder…** and choose **Add to favorites** from the menu on the folder name at the bottom of the sidebar. The folder Olive opened first is already there. Your favorite folders are listed in that menu from then on.

## Daily notes

Click the **Daily notes** row at the top of the sidebar, or press `⌥⌘N` (**Go ▸ Today's Note**), to open today's note. It is created if it does not exist yet, at `Daily/2026/10/2026-10-06.md` for 6 October 2026.

Daily notes are on whenever the folder has a top-level folder named `Daily`. Olive creates one in the folder it sets up for you on first launch. To turn daily notes on or off elsewhere, use **Daily notes** in Settings; turning them off moves the `Daily` folder and its notes to the Trash, from where **Recently Deleted** can bring them back.

## Getting around

- **Back** and **Forward** — `⌘[` and `⌘]`, the arrows at the top left of the note, or a two-finger swipe on the trackpad.
- **Go to the enclosing folder** — the up arrow beside them, or **Go ▸ Enclosing Folder**.
- **Home** — click the folder name at the bottom of the sidebar.

## Go to Note and search

Press `⌘P` (or `⇧⌘F`), or click the magnifier at the top of the sidebar, and type. Before you type, the panel lists the notes you opened recently. As you type, it lists the notes whose names match, then, under **In notes**, the notes whose text contains what you typed, each with one matching line and the number of matches. The search of the text ignores case. Use `↑` `↓` and `Enter`, or click: a name opens the note from the top, and a text match opens the note at that place. `⌘Enter` opens it in a new window. `Esc` closes the panel.

Notes stored in iCloud Drive that are not downloaded to this Mac are downloaded to be searched, and the result says how many.

To search within the open note instead, press `⌘F`.

## Outline

The headings of the open note are listed under it in the sidebar. Click a heading to jump to it, or drag it to move the whole section. Right-click a heading to **Promote** or **Demote** it, **Select section**, or choose how many levels to show. The arrow on the note's row, or **View ▸ Hide Outline**, hides or shows the outline.

---

Back to the [contents](README.md).
