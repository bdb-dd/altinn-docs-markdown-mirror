# Altinn docs Markdown mirror

A weekly GitHub Pages build of [docs.altinn.studio](https://docs.altinn.studio/) that also emits a Markdown copy of every page and a Markdown sitemap, for ingestion by retrieval tools.

- **Content:** current `Altinn/altinn-studio-docs` master, merged at build time into
  [`bdb-dd/altinn-studio-docs@markdown-mirror`](https://github.com/bdb-dd/altinn-studio-docs/tree/markdown-mirror),
  which carries the Markdown output formats from [Altinn/altinn-studio-docs#2484](https://github.com/Altinn/altinn-studio-docs/pull/2484).
- **Entry point:** `sitemap-markdown.xml` (a sitemap index of the `en` and `nb` Markdown sitemaps). Each page is at `<page>/index.md`.
- **Schedule:** Mondays 01:00 UTC, plus manual runs (`workflow_dispatch`).
- If upstream stops merging cleanly, the run fails and names the conflicting files; resolve them on the `markdown-mirror` branch.

The canonical site is docs.altinn.studio; cite that, not this mirror. Once #2484 is merged upstream, this repository is no longer needed.
