# FAQ

## Is Olive open source?

No. Olive is closed source, and this repository contains no extension source. It exists
so that documentation and issue tracking are public.

## Does Olive change my Markdown files?

Only where you edit. Constructs Olive cannot edit as rich text are kept verbatim and
shown as an explicit source block, so nothing is silently dropped or rewritten. A file
you open and save without editing is byte-identical to what it was.

## Does Olive take over `.md` files?

No. VS Code's text editor stays the default and you opt in per file, through
**Open in Olive** or **Reopen Editor With…**. You can make Olive the default yourself
with `workbench.editorAssociations`; see the Marketplace page.

## How is this different from VS Code's built-in Markdown Editor (Experimental)?

Both let you edit rendered Markdown. Olive is aimed at *technical* documents: TeX math
rendered with KaTeX and re-editable in a dedicated input surface, tables you manipulate
as structure, callouts, toggles and Mermaid diagrams that stay editable, and syntax
markers that stay hidden even inside the element the cursor is in. The two can coexist —
installing Olive does not affect the built-in editor.

## Does Olive send anything anywhere?

No. No network requests, no telemetry, no analytics. See "Data handling" in the
[README](README.md#data-handling).

## Which Markdown dialect does Olive use?

CommonMark plus GitHub Flavored Markdown (tables, task lists, strikethrough), with
`$…$` / `$$…$$` for math. Callouts use the blockquote-with-marker form. Anything Olive
does not recognise is preserved verbatim rather than reformatted.

## Does it work over SSH, WSL, Dev Containers or Codespaces?

Untested in this release. It may work, but nothing has been verified. Untrusted
workspaces and virtual workspaces are explicitly not supported and Olive stays disabled
in them.

## Is it free? Will it stay free?

It is free during preview. If a future version is offered for a fee, versions that were
distributed free of charge remain usable free of charge — see
[LICENSE-extensions](LICENSE-extensions) §2.

## Are the Mac and iOS apps available?

Not yet. The VS Code extension shipped first. When the apps arrive, they will use this
same repository for issues.

## Where is the changelog?

On the extension's
[Marketplace Changelog tab](https://marketplace.visualstudio.com/items?itemName=mohashi.olive&ssr=false#version-history).
It is deliberately not duplicated here, so there is only one copy to keep correct.
