## Privacy Policy

**Last updated: 2026-10-21**

Olive is a Markdown editor for macOS, iOS, and Visual Studio Code, developed by Mohashi.

### Summary

**Olive does not collect any data.** There are no accounts, no analytics, and no crash reporting. Your notes stay on your device and in the folder you choose. The macOS app checks for its own updates; nothing else goes online unless you ask for it.

### What Olive stores

- **Your notes** are plain `.md` files in a folder you pick. Olive never moves them anywhere you did not choose.
- **Local application data** — unsaved drafts, the file recovery history, your theme, and your window and sidebar preferences — is stored on your device only, in the app's own storage. Deleting the app deletes it.
- If you keep your folder in iCloud Drive, Google Drive, or another file-syncing service, that service syncs the files as it would for any other folder on your device. Olive is not involved in that transfer, and the service's own privacy policy applies.

### Network access

The macOS app contacts a server on its own in one case only: to check whether a newer version of Olive has been released. Every other request below happens only when you start it.

- **Checking for updates (macOS app only)** — the macOS app is distributed directly rather than through the Mac App Store, so it checks GitHub for a newer version shortly after it starts and once a day while it stays open. The request carries no information about you or your notes; GitHub sees it and your IP address, as it would for any download. If a newer version is available, Olive downloads and installs it quietly, and the new version is used the next time you open Olive — it never interrupts you to ask. You can also check at any time with **Olive ▸ Check for Updates…**. The iOS app updates through the App Store and the Visual Studio Code extension through the Marketplace, so neither of them makes this request.
- **Import from Notion (macOS only)** — when you paste a Notion API token and start an import, Olive contacts Notion's API and the attachment URLs it returns, in order to download your pages. The token is used for that import and is not sent anywhere else.
- **Connecting Google Drive (browser version only)** — if you connect a Google account in the browser version, Olive uses Google's sign-in to read and write the files you select. This is not available in the macOS or iOS apps.
- **Images and links you put in your notes** — if a note references an image on the web (an `https://` URL), your device fetches that image to display it, exactly as a web browser would, and again when you copy it with **Copy image**. The image's host sees that request. Images stored in your folder never leave it.
- **The PDF engine (Visual Studio Code extension only)** — if Olive cannot find a Chromium-based browser on your computer for PDF export, it offers to download a print-only engine. It is downloaded only if you accept that prompt, or if you run **Olive: Update PDF engine**.

### What Olive never does

- No analytics, telemetry, usage statistics, or advertising identifiers.
- No crash reporting.
- No account, sign-up, or login for Olive itself.
- Your notes are never sent to Mohashi or to any third party.

### Children

Olive is not directed at children and collects no personal information from anyone, including children.

### Changes to this policy

If this policy changes, the updated version will be posted at this URL with a new "Last updated" date.

### Contact

Questions and reports: https://github.com/mohashii/olive-feedback/issues
