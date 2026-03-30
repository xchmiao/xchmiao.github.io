# xchmiao.github.io

Minimal Astro blog for technical posts.

## Local development

```bash
npm install
npm run dev
```

## Build for GitHub Pages

```bash
npm run build
```

Astro outputs the static site to `docs/`.

## Writing

Create new posts in `src/content/posts/`:

```md
---
title: "A concrete technical lesson"
description: "One sentence on what the post covers."
date: 2026-03-30
tags:
  - engineering
  - notes
draft: false
---
```

## GitHub Pages setup

This repo is set up to follow GitHub Pages branch deployment:

1. Push the repository to GitHub as `xchmiao.github.io`.
2. In GitHub, open `Settings` -> `Pages`.
3. Under `Build and deployment`, set `Source` to `Deploy from a branch`.
4. Set the branch to `main` and the folder to `/docs`.
5. Run `npm run build` and commit the generated `docs/` folder whenever you publish changes.

This matches GitHub's Pages quickstart flow for a user site, while still letting you author the site in Astro.
