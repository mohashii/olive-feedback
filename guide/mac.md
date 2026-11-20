# Olive for Mac

Olive for Mac edits a folder of Markdown files. The files on your disk are the originals: Olive edits them in place, so any other editor, a sync service or Git can work with the same folder.

## Your first folder

The first time Olive starts on a Mac with iCloud Drive, it creates a folder named **Olive** in iCloud Drive and opens it, with a short **Welcome to Olive** note. If a folder named Olive is already there — from another Mac, for example — it opens that one instead. A message tells you where your notes are being saved.

To work in a different folder, such as an existing Obsidian vault, click the folder name at the bottom of the sidebar, open the menu with the ⌃⌄ beside it, and choose **Open another folder…** (or **File ▸ Open Folder…**, `⌘O`). Olive opens the last folder again the next time it starts. Without iCloud Drive, Olive starts with an **Open folder…** button instead.

## The window

**The sidebar** lists the folder's notes and subfolders.

- Beside the window buttons are the sidebar toggle (`⌃⌘S`), **Go to Note** (`⌘P`) and **New note** (`⌘N`).
- At the bottom, the folder's name takes you to its home page. The ⌃⌄ beside it opens a menu with your favorite folders, **Add to favorites**, **Open another folder…**, **Refresh files**, **Export as HTML…**, **Recently Deleted…**, **Settings…** and **Help**. At the right end of that row is **Collapse all**.
- Drag the sidebar's edge to make it wider or narrower. Olive remembers the width, and whether the sidebar is hidden.

**The note** takes the rest of the window. At its top left are **Go to the enclosing folder**, **Back** (`⌘[`) and **Forward** (`⌘]`); swiping left or right with two fingers on the trackpad also goes back and forward. Its header stays quiet while Olive saves by itself and speaks up when something needs you (see [Saving and recovery](saving-and-recovery.md#how-olive-saves)). Its **…** menu holds the actions for this note: **Find in document**, **Document info**, **Save now**, **Auto-save**, **File name follows title**, **File recovery…**, **Add property** (`⌘;`), **Change icon…**, **Reveal in Finder** and **Copy path**.

How to work with the files themselves is in [Folders and notes](folders-and-notes.md), and how saving works in [Saving and recovery](saving-and-recovery.md).

## Several windows

**File ▸ New Window** (`⇧⌘N`) opens another window on the same folder. **Open in new window** on a note or folder in the sidebar opens that one in its own window, and so does `⌘Enter` in **Go to Note**. Each window can open a different folder.

Closing the last window leaves Olive running; click its icon in the Dock to open a new window. Olive reopens its first window where you left it.

## Opening a single file

Olive can open a Markdown file that is not in your folder. Choose **File ▸ Open File…**, or choose Olive from **Open With** on a `.md` file in Finder. If a window already has the folder that holds the file open, the file opens there; if one of your favorite folders holds it, Olive opens that folder in a new window; otherwise the file opens in a window of its own.

## Settings

**Olive → Settings…** (`⌘,`) applies changes as you make them.

| Setting | What it does |
| --- | --- |
| Body text size in notes | Default, Large, Larger or Largest. The sidebar keeps its size |
| Sidebar size | Small, Medium or Large: the size of the rows and text in the sidebar |
| Show other files | Lists files that are not Markdown — pictures, PDFs and so on — in the sidebar. On by default |
| What to add to the end of an exported HTML file | See [Export](export.md#in-the-mac-app) |
| Daily notes | Turns daily notes on or off for this folder; see [Daily notes](folders-and-notes.md#daily-notes) |

Daily notes are a property of the folder, so every Mac that opens it follows the same choice. The other settings belong to this Mac.

## Appearance

Olive follows the macOS appearance, light or dark.

**View ▸ Zoom In** (`⇧⌘.`), **Zoom Out** (`⇧⌘,`) and **Actual Size** (`⇧⌘0`) make the note larger or smaller — text, pictures and margins together — while the sidebar stays the same. The zoom applies to every window and is kept the next time Olive starts. **Body text size** in Settings changes only the size of the text.

---

Back to the [contents](README.md).
