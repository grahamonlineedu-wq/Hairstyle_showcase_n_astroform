# Crown & Canvas

An Astro-powered beauty and style journal featuring textured hairstyles, men's grooming, nail art, and wigs and extensions. The site is built as a static blog with Markdown and MDX content collections.

## Run locally

```sh
npm install
npm run dev
```

Create a production build with:

```sh
npm run build
npm run preview
```

## Add a journal story

Add a `.md` or `.mdx` file to `src/content/blog/` with the required frontmatter:

```yaml
---
title: 'Story title'
description: 'A short summary for the lookbook and search results.'
category: 'Hair'
pubDate: '2026-10-26'
heroImage: '../../assets/your-cover-image.jpg'
heroImageAlt: 'A concise description of the cover image'
---
```

Supported categories include Hair, Grooming, Nail art, Hair units, and Studio notes. Local images in `src/assets/` are optimized by Astro during the build.

## Deployment URL

Before publishing, replace the `site` value in `astro.config.mjs` with the public URL. Astro uses it to generate canonical URLs, the sitemap, and absolute feed links.
