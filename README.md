# LPD-106049 · Structure Builder — Search Settings

Prototype for the **Advanced** tab of CMS Content Structure fields, replacing today's technical *Keyword vs Text* choice.

**Live:** https://mariaarcevich.github.io/LPD-106049-Structure-Builder-Search-Settings/

## What it shows

Two proposals, switchable from the prototype controls (bottom right):

1. **Searchable + Filterable** — two independent checkboxes (Text form / Keyword form) with defaults by field type. Intermediate step for [LPD-106049](https://liferay.atlassian.net/browse/LPD-106049): changes still need a reindex, so the flow warns when an option is removed, confirms on publish, and after publishing shows the next step (link to Index Actions for admins, "ask an administrator" otherwise) plus a **Reindex Pending** label on the structure.
2. **Always Index Both** — a single **Searchable** checkbox; the search framework always indexes both forms and catches up existing content in the background, so no manual reindex is needed. Target of the Search spike ([LPD-106265](https://liferay.atlassian.net/browse/LPD-106265)).

Both proposals remove the per-field language selector and the per-field AI search option.

Prototype settings: **Structure Published** and, for proposal 1, **User Can Reindex**.

Built with [Lexicon Vanilla](https://liferay-design.github.io/lexicon-vanilla/) components (CMS style). Opens directly in the browser, no build.
