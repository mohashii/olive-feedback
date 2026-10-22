# Import from Notion

The Mac app can bring a Notion page, and every page below it, into a folder of Markdown notes. The import only reads from Notion; nothing there is changed.

## Before you start

You need a Notion token that can read the page: a personal access token, or the token of an internal integration that the page is shared with. **How to create a token** in the import window opens Notion's integrations page. Olive does not save the token; it forgets it when the import window closes.

## Importing

1. Choose **File → Import from Notion…** and paste the token.
2. Paste the URL of the Notion page to import, copied from Notion, and click **Check contents**. Olive counts the pages and attachments.
3. Choose where to put the import with **Choose folder…**, and name the new folder. Olive creates that one folder and writes everything inside it; existing folders are left untouched.
4. Click **Import**.

Notion limits how fast pages can be read, so a large import can take several minutes. You can quit Olive in the middle: starting the same import again picks up where it stopped. **Stop** ends it early.

## What you get

- The page you chose becomes the folder note (`index.md`) of the new folder. A page with subpages becomes a folder of its own, with the page as that folder's note.
- Attachments and images are saved in an `assets` folder beside the page that uses them.
- Anything Olive could not bring over, such as a database or an embed it could not fetch, is marked in the note with a warning, usually with a link to the original block in Notion.
- When the import finishes, Olive says how many pages and attachments it brought in and whether anything needs your review. **Open the report** opens `Notion import report.md`, a note at the top of the imported folder that lists the imported pages and those items. **Open in Olive** switches to the imported folder.

Importing contacts Notion's servers, using your token; see the [privacy policy](https://github.com/mohashii/olive-feedback/blob/main/PRIVACY.md#network-access).

---

Back to the [contents](README.md).
