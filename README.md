# Olive

**This is not the source repository for Olive.** Olive is closed source. This repository
exists so that documentation and issue tracking are public: the FAQ, troubleshooting
notes, and the issue tracker where bugs, feature requests and questions are handled.

Olive lets you write Markdown without seeing the syntax. Formatting stays visible even under the cursor — headings, rich text, code, TeX math, tables and structured blocks — while the file on disk stays plain Markdown.

![A learning log opened as Markdown source in VS Code, switched to Olive, and edited visually: bold text, inline code and inline math form from typed Markdown; the formula updates while its LaTeX is edited in a popup; a Mermaid diagram renders; a table column moves from its right-click menu; and the file returns to plain Markdown source](media/olive-hero.gif)

## Where to get it

| Platform | Status |
| --- | --- |
| **VS Code extension** | [Olive — Visual Markdown Editor on the Marketplace](https://marketplace.visualstudio.com/items?itemName=mohashi.olive-markdown) |
| Mac, iPad, iPhone apps | In development, not released |

Full documentation for the VS Code extension — supported blocks, keyboard shortcuts, how to open a file in Olive, exporting to HTML and PDF — lives on its [Marketplace page](https://marketplace.visualstudio.com/items?itemName=mohashi.olive-markdown).

## Reporting something

Open an issue: **[Bug report](https://github.com/mohashii/olive-feedback/issues/new?template=bug_report.yml)** ·
**[Feature request](https://github.com/mohashii/olive-feedback/issues/new?template=feature_request.yml)** ·
**[Question](https://github.com/mohashii/olive-feedback/issues/new?template=question.yml)**

Bug reports are most useful when they include **the Markdown that broke** — malformed
output, math that renders wrong, or a conflict with another extension. A minimal
snippet that reproduces it is worth more than a description of it.

Two things do not belong in a public issue:

- **Confidential documents.** Reduce the file to a minimal snippet that still
  reproduces the problem, and strip anything you would not publish.
- **Security vulnerabilities.** See [SECURITY.md](SECURITY.md) for the private channel.

Before opening a bug, [TROUBLESHOOTING.md](TROUBLESHOOTING.md) covers the failures that
turn out to have a local cause. [FAQ.md](FAQ.md) covers what Olive does and does not do.

## Data handling

Olive collects no telemetry and has no analytics of any kind — this issue tracker is the only way problems reach the author, which is why reports matter. It reads and writes the Markdown files and images in your workspace, through VS Code's own document APIs, plus the HTML and PDF files you export.

Olive itself makes one network request, and only if you ask for it: downloading the PDF print engine, after you accept the prompt it shows when it cannot find a Chromium-based browser on your machine. Separately, images that a document references by an `https://` URL are loaded for display, as they would be in any Markdown preview. Nothing else goes online.

## Changelog

Version history is on the extension's
[Marketplace Changelog tab](https://marketplace.visualstudio.com/items?itemName=mohashi.olive-markdown&ssr=false#version-history).
It is not duplicated here.

## Licence

The Olive extension is proprietary. The end user licence agreement it ships with is
mirrored here as [LICENSE-extensions](LICENSE-extensions) for reference; the copy inside
the installed extension governs. Bundled open-source components and their licences are
listed in the THIRD-PARTY-NOTICES.md file included with the extension.
