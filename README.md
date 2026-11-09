# Next.js Static Blog

A lightweight static blog built with Next.js (Pages Router) demonstrating Static Site Generation (SSG) from local Markdown files.

**Live Demo:** https://nextjs-blog-theta-amber-95.vercel.app/

## Overview

This project was built to practice core Next.js Pages Router concepts:
- Pre-rendering via Static Site Generation (`getStaticProps` and `getStaticPaths`).
- Dynamic routing for Markdown content (`pages/posts/[id].js`).
- Client-side page transitions and prefetching with `next/link`.
- Scoped styling using CSS Modules and global styles via `_app.js`.

## Tech Stack

- **Framework:** Next.js (Pages Router)
- **Library:** React
- **Content:** Markdown parsed with `gray-matter`, `remark`, and `remark-html`
- **Utilities:** `date-fns`
- **Hosting:** Vercel

## Project Structure

```text
├── components/          # Reusable UI components (Layout, Date)
├── lib/                 # Node.js file system logic & Markdown parsers
├── pages/
│   ├── posts/
│   │   └── [id].js      # Dynamic route for blog posts
│   ├── _app.js          # Custom App for global CSS injection
│   └── index.js         # Blog listing homepage
├── posts/               # Raw Markdown files (.md)
├── public/              # Static files (images, icons)
└── styles/              # Global and modular CSS stylesheets