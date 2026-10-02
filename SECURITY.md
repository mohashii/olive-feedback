# Security policy

## Reporting a vulnerability

**Do not open a public issue for a security problem.**

Use GitHub's private vulnerability reporting instead:
[Report a vulnerability](https://github.com/mohashii/olive-feedback/security/advisories/new). The report is visible only to
you and the author until a fix is published.

Olive collects no telemetry, and the few cases in which it goes online are listed under "Data handling" in the [README](README.md#data-handling). The interesting surface is therefore mostly local: what the extension does with the contents of the files it opens; with links, images (including those a document references by `https://` URL) and embedded content inside a document; and with the HTML and PDF files it exports. The PDF engine download is in scope too.

Please include what an attacker would need to control (a crafted Markdown file, a
workspace setting, a linked resource), what they gain, and a minimal document that
demonstrates it. Do not attach documents containing real confidential data.

## Scope

This policy covers the Olive VS Code extension. Vulnerabilities in VS Code itself belong
to [Microsoft](https://github.com/microsoft/vscode/blob/main/SECURITY.md), and
vulnerabilities in a bundled open-source component are best reported upstream as well —
tell us either way so the bundled version can be updated.
