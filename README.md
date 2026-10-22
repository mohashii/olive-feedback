# Olive

**This is not the source repository for Olive.** Olive is closed source. This repository
exists so that documentation and issue tracking are public: the [user guide](guide/README.md),
and the issue tracker where bugs, feature requests and questions are handled.

Olive lets you write Markdown without seeing the syntax. Formatting stays visible even under the cursor — headings, rich text, code, TeX math, tables and structured blocks — while the file on disk stays plain Markdown.

![A learning log opened as Markdown source in VS Code, switched to Olive, and edited visually: bold text, inline code and inline math form from typed Markdown; the formula updates while its LaTeX is edited in a popup; a Mermaid diagram renders; a table column moves from its right-click menu; and the file returns to plain Markdown source](media/olive-hero.gif)

## Where to get it

| Platform | Status |
| --- | --- |
| **Mac** | [Download from Releases](https://github.com/mohashii/olive-feedback/releases/latest) — macOS 13.3 or later, Apple Silicon and Intel |
| **VS Code extension** | [Olive — Visual Markdown Editor on the Marketplace](https://marketplace.visualstudio.com/items?itemName=mohashi.olive-markdown) |
| iPad and iPhone apps | In development, not released |

How to use Olive — on the Mac and in VS Code — is in the **[user guide](guide/README.md)**: blocks, keyboard shortcuts, folders and saving on the Mac, opening a file in Olive in VS Code, exporting to HTML and PDF.

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

Before opening a bug, [Troubleshooting](guide/troubleshooting.md) covers the failures that
turn out to have a local cause. The [FAQ](guide/faq.md) covers what Olive does and does not do.

## Data handling

Olive collects no telemetry and has no analytics of any kind — this issue tracker is the only way problems reach the author, which is why reports matter. It does not send your documents anywhere. The few cases in which it goes online at all are listed under "Network access" in the [privacy policy](PRIVACY.md#network-access). The files the VS Code extension reads and writes are listed in section 5 of the [licence](LICENSE-extensions).

## Changelog

The Mac app's release notes are on [Releases](https://github.com/mohashii/olive-feedback/releases). The VS Code extension's version history is on its
[Marketplace Changelog tab](https://marketplace.visualstudio.com/items?itemName=mohashi.olive-markdown&ssr=false#version-history).

## Licence

The Olive extension is proprietary. The end user licence agreement it ships with is
mirrored here as [LICENSE-extensions](LICENSE-extensions) for reference; the copy inside
the installed extension governs. Bundled open-source components and their licences are
listed in the THIRD-PARTY-NOTICES.md file included with the extension.
