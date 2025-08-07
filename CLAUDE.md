# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Slidev-based presentation project titled "AI is Here" focused on introducing AI tools and workflows for Product Engineering Teams. Slidev is a Vue.js-based presentation framework that uses Markdown for slide content with Vue component support.

## Source Control
- Always use feature branches
- Github CLI is installed, after pushing always open a PR

## Development Commands

- `pnpm install` - Install dependencies (required first step)
- `pnpm dev` - Start development server at http://localhost:3030
- `slidev build` - Build production version of slides
- `slidev export` - Export slides to PDF or other formats

## Architecture

The project follows Slidev's standard structure:

- `slides.md` - Main presentation content in Markdown with frontmatter configuration
- `components/` - Vue components (e.g., Counter.vue) that can be used within slides
- `snippets/` - TypeScript code snippets that can be imported into slides using `<<< @/snippets/filename.ts#region`
- `pages/` - Additional slide pages that can be imported via `src:` directive

## Presentation Content Structure

The presentation covers AI integration in software engineering with sections on:
- Personal background and experience
- AI characteristics and limitations
- Practical examples (code reviews, testing, debugging, learning)
- Recommendations for adoption

## Key Features in Use

- Seriph theme with custom styling
- Vue component integration (Counter component example)
- External code snippet imports with region support
- Slide transitions and animations
- Monaco editor integration for live code examples

## Deployment

Configured for both Netlify (netlify.toml) and Vercel (vercel.json) deployment.

## Working with Slides

- Edit `slides.md` for main content
- Use frontmatter `---` blocks for slide configuration
- Vue components in `components/` are auto-imported
- Code snippets support syntax highlighting and line highlighting with `{lines}` syntax
- Use `v-click` for click animations and `v-motion` for motion animations