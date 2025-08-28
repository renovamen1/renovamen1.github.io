# Project Overview

This is a personal website built with [Astro](https://astro.build/), [Solid](https://www.solidjs.com/) and [UnoCSS](https://github.com/antfu/unocss). The website serves as a personal portfolio and blog.

## Key Technologies

*   **Framework:** [Astro](https://astro.build/) - A modern static site builder.
*   **UI Framework:** [SolidJS](https://www.solidjs.com/) - A declarative JavaScript library for building user interfaces.
*   **Styling:** [UnoCSS](https://github.com/antfu/unocss) - An instant on-demand atomic CSS engine.
*   **Package Manager:** [pnpm](https://pnpm.io/)

## Project Structure

*   `src/`: Contains the main source code for the website.
    *   `components/`: Reusable Astro and SolidJS components.
    *   `content/`: Markdown files for blog posts, projects, and other content.
    *   `layouts/`: Astro layouts for different page types.
    *   `pages/`: Astro pages that define the routes of the website.
    *   `styles/`: CSS files for global styles and fonts.
    *   `utils/`: Utility functions for posts, tags, and other functionalities.
*   `public/`: Static assets such as images, fonts, and a CNAME file.
*   `plugins/`: Custom remark and rehype plugins for markdown processing.
*   `astro.config.ts`: Astro configuration file.
*   `unocss.config.ts`: UnoCSS configuration file.
*   `package.json`: Defines the project's dependencies and scripts.

# Building and Running

## Prerequisites

*   [Node.js](https://nodejs.org/) (v18 or higher)
*   [pnpm](https://pnpm.io/)

## Development

To start the development server, run the following command:

```bash
pnpm dev
```

## Build

To build the website for production, run the following command:

```bash
pnpm build
```

The output will be in the `dist/` directory.

## Linting

To lint the codebase, run the following command:

```bash
pnpm lint
```

# Development Conventions

## Markdown

The website uses a highly customized markdown processing pipeline with remark and rehype plugins. These plugins add support for features like:

*   Table of contents
*   Code blocks with syntax highlighting
*   Math equations (KaTeX)
*   Custom containers
*   Autolinking headings

The configuration for these plugins can be found in `plugins/index.ts`.

## Styling

The website uses [UnoCSS](https://github.com/antfu/unocss) for styling. The configuration can be found in `unocss.config.ts`. It includes:

*   **Shortcuts:** Pre-defined utility combinations for common UI patterns.
*   **Theme:** A custom theme with light and dark mode support.
*   **Presets:** A set of presets for common CSS utilities.

## Content

All content is written in Markdown and located in the `src/content/` directory. The content is organized into collections, such as `blog`, `projects`, and `publications`.
