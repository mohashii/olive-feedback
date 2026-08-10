# Olive

**This is not the source repository for Olive.** Olive is closed source. This repository
exists so that documentation and issue tracking are public: the FAQ, troubleshooting
notes, and the issue tracker where bugs, feature requests and questions are handled.

Olive lets you edit technical Markdown like a document — headings, rich text, code, TeX
math, tables and structured blocks — without stopping to manage syntax. The file on disk
stays plain Markdown.

![Create a technical document, format text, select and move multiple blocks, edit Markdown source and render a Mermaid diagram](media/olive-demo.gif)

## Where to get it

| Platform | Status |
| --- | --- |
| **VS Code extension** | [Olive Markdown Editor on the Marketplace](https://marketplace.visualstudio.com/items?itemName=mohashi.olive) — preview |
| Mac, iPad, iPhone apps | In development, not released |

Full documentation for the VS Code extension — supported blocks, keyboard shortcuts,
how to open a file in Olive — lives on its
[Marketplace page](https://marketplace.visualstudio.com/items?itemName=mohashi.olive).

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

Olive makes no network requests and collects no telemetry. It reads and writes only the
Markdown files and referenced local images in your workspace, through VS Code's own
document APIs. There is no analytics of any kind — this issue tracker is the only way
problems reach the author, which is why reports matter.

## Changelog

Version history is on the extension's
[Marketplace Changelog tab](https://marketplace.visualstudio.com/items?itemName=mohashi.olive&ssr=false#version-history).
It is not duplicated here.

## Licence

The Olive extension is proprietary. The end user licence agreement it ships with is
mirrored here as [LICENSE-extensions](LICENSE-extensions) for reference; the copy inside
the installed extension governs. Bundled open-source components and their licences are
listed in the THIRD-PARTY-NOTICES.md file included with the extension.
