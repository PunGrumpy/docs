# Agent guide

This repository is the Mintlify source for <https://pungrumpy.mintlify.app>, a reference edition of the
portfolio at <https://pungrumpy.com>.

## Ground rules

1. **The portfolio is canonical.** If a fact here disagrees with pungrumpy.com, the portfolio wins. Check
   <https://www.pungrumpy.com/llms.txt> before changing dates, project descriptions, or job titles.
2. **Do not invent evidence.** Credentials require a public verification URL. Projects require a real
   repository or live URL. Omit rather than guess.
3. **Design is constrained.** Composition follows <https://vercel.com/design.md> and is summarised in
   `reference/colophon.mdx`. Monochrome only, no card grids, no metric tiles, no badges around ordinary
   metadata, no decorative motion. Prefer tables for lookup and prose for argument.
4. **Navigation is explicit.** A new page must be added to the `navigation` groups in `docs.json` or it
   will not appear.

## Conventions

- Frontmatter carries `title` and `description` on every page; add `sidebarTitle` when the title is long.
- Headings are sentence case. No em dashes in headings.
- Prose stays within a readable measure; long lists of facts become tables.
- Internal links use absolute paths without the extension, for example `/projects/pigo`.

## Verifying a change

```bash
mint dev
```

Check the page renders, the sidebar entry appears, and every link resolves.
