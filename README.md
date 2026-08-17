# docs

Documentation site for [pungrumpy.com](https://pungrumpy.com), published at
**[pungrumpy.mintlify.app](https://pungrumpy.mintlify.app)**.

A reference edition of the portfolio: profile, work history, projects, writing, and credentials, written
to be scanned by people and read whole by agents. The portfolio remains canonical; this site summarises
it and links back.

## Stack

- [Mintlify](https://mintlify.com), configured in `docs.json`
- Geist for headings and body
- Monochrome palette, composition following the
  [Vercel brand design guidelines](https://vercel.com/design.md)

## Local development

```bash
npm i -g mint
mint dev
```

Opens on `http://localhost:3000`.

## Layout

```
docs.json                 site config, navigation, theming
style.css                 restraint layer: measure, tabular numerals, table alignment
index.mdx                 overview
profile.mdx               identity, focus areas, contact
stack.mdx                 languages, frameworks, infrastructure
experience.mdx            work history
education.mdx             academic background
achievements.mdx          programs and certifications, with verification links
projects/                 catalogue plus one page per project
writing/                  index of published posts
reference/discovery.mdx   machine-readable entry points on pungrumpy.com
reference/colophon.mdx    how this site is built and why
```

## Editing rules

- Facts that disagree with [pungrumpy.com](https://pungrumpy.com) are resolved in favour of the portfolio.
- Credentials are listed only with a public verification link.
- Design decisions follow `reference/colophon.mdx`. Read it before adding a component.

## Deployment

Pushes to `main` deploy automatically through the Mintlify GitHub integration.
